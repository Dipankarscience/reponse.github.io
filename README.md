# Responsive-website
Its a responsive website created using html and css only by using media quires and keyframes and all to give it a nice look and animation. And other basics stuffs also have been used.



<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Educational responsive Website by Dipankar</title>
    <link href="https://fonts.googleapis.com/css2?family=Merienda+One&family=Noto+Serif:ital@1&display=swap"
        rel="stylesheet">
    <style>
        /* CSS Reset  */
        * {
            margin: 0px;
            padding: 0px;
            scroll-behavior: smooth;
        }
        body{
            background-color: rgba(0, 0, 0, 0.192);
        }
        /* Nav bars section  */
        #navbars {
            display: flex;
            padding: 5px;
            background: black;
            opacity: 0.75;
            flex-wrap: wrap;
            position: sticky;
            top: 0;
            left: 0;
            margin: 0;
            /* width: 100vw; */
        }

        #navbars img {
            height: 72px;
            width: 100px;
        }

        #navbars ul {
            display: flex;
            margin: 10px 12px;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
        }

        #navbars ul li {
            margin: 10px 16px;
            list-style: none;
            padding: 5px;
            animation: animone 6s ease-in-out 4s infinite forwards;
        }
        /* Animation  */
        @keyframes animone{
            0%{
                background-color: royalblue;
                
                border-radius: 4px;
            }
            25%{
                background-color: salmon;
                border-radius: 4px;
            }
            50%{
                background-color: snow;
                border-radius: 4px;
            }
            75%{
                background-color: brown;
            }
            100%{
                background-color: burlywood;
                border-radius: 4px;
            }
        }
        #navbars ul li a {
            text-decoration: none;
            text-align: center;
            font-size: 1.18rem;
            font-family: 'Noto Serif', serif;
            color: black;
            font-weight: bolder;
        }

        /* Home section  */
        #Home {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            margin: 0px;
            /* width: 100vw; */
        }

        #Home #head {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            margin: 22px 15px;
            padding: 15px;
            flex-wrap: wrap;
        }

        #Home #head h1 {
            margin: 6px;
            padding: 5px;
            font-size: 2.8rem;
            font-family: 'Merienda One', cursive;
            text-align: center;
            font-weight: bolder;
        }

        #Home #head p {
            margin: 3px;
            padding: 5px;
            font-size: 1.3rem;
            font-family: 'Noto Serif', serif;
            text-align: center;
            font-weight: bolder;
        }

        /* Before home  */
        #Home ::before {
            position: absolute;
            content: "";
            top: 0;
            left: 0;
            background: url('https://cdn.pixabay.com/photo/2015/07/02/10/38/stairway-828883_960_720.jpg') no-repeat center center/cover;
            height: 50%;
            width: 100vw;
            z-index: -1;
            opacity: 0.5;
            margin: 0;
        }

        /* Courses section  */
        #Courses {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            flex-wrap: wrap;
            margin-top: 90px;
            margin-bottom: 80px;
            margin-right: 0px;
            margin-left: 0px;
            width: 100%;
            /* height: 100%; */
        }

        #Courses #course {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin: 22px 0px;
            padding: 0px;
            flex-wrap: wrap;
            width: 100vw;
            height: 100%;
        }

        #Courses #course h2 {
            margin: 6px;
            padding: 5px;
            font-size: 2.8rem;
            font-family: 'Merienda One', cursive;
            text-align: center;
            font-weight: bolder;
        }

        #Courses #course #subject {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            width: 70vw;
            flex-direction: column;
            
        }

        #Courses #course #subject .subjects {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            border: 2px solid rgb(122, 30, 30);
            background: rgb(241, 189, 189);
            flex-direction: column;
            margin: 6px 15px;
            border-radius: 10px;
            animation: animtwo 6s ease-in-out 4s infinite forwards;
            cursor: pointer;
        }
        @keyframes animtwo{
            0%{
                background-color: cornsilk;
            }
            25%{
                background-color: cyan;
            }
            50%{
                background-color: darkkhaki;
            }
            75%{
                background-color: coral;
            }
            100%{
                background-color: rgb(92, 78, 182);
            }
        }
        
        #Courses #course #subject .subjects :hover{
            background-color: indianred;
            border-radius: 5px;
        }

        #Courses #course #subject .subjects h3 {
            margin: 5px;
            padding: 5px;
            text-align: center;
            font-size: 1.7rem;
            font-family: 'Merienda One', cursive;
            font-weight: bolder;
        }

        #Courses #course #subject .subjects p {
            margin: 5px;
            padding: 10px;
            text-align: center;
            font-size: 15px;
            font-family: 'Noto Serif', serif;
            font-weight: bolder;
        }

        #Courses #course #subject .subjects img {
            margin: 2px;
            height: 72px;
            width: 90px;
        }

        /* Faculties section  */
        #Faculties {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            position: relative;
            height: auto;
            width: 100%;
            margin: 10px 0px;
            top: 0;
            left: 0;
        }

        #Faculties div {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
        }

        #Faculties ::before {
            position: absolute;
            content: "";
            top: 0;
            left: 0;
            background: url('https://cdn.pixabay.com/photo/2017/06/17/06/08/laptop-2411303_960_720.jpg') no-repeat center center/cover;
            height: 100%;
            width: 100%;
            z-index: -1;
            opacity: 0.5;
        }

        #Faculties div h2 {
            margin: 10px;
            padding: 5px;
            font-size: 2.4rem;
            text-align: center;
            font-family: 'Merienda One', cursive;
            font-weight: bolder;
        }

        #Faculties div p {
            margin: 20px;
            padding: 15px;
            font-size: 1.3rem;
            text-align: center;
            font-family: 'Noto Serif', serif;
        }

        /* Enroll section  */
        #Enroll {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            position: relative;
            margin-top: 100px;
            margin-bottom: 0px;
            margin-right: 0px;
            margin-left: 0px;
            height: auto;
            width: 100%;
            top: 0;
            left: 0;
        }

        #Enroll #formgr {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            width: 100%;
        }

        #Enroll #formgr form {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            /* overflow: hidden; */
        }

        #Enroll ::before {
            position: absolute;
            content: "";
            background: url('https://cdn.pixabay.com/photo/2019/10/05/11/15/school-4527713_960_720.jpg') center center/cover;
            top: 0;
            left: 0;
            z-index: -1;
            opacity: 0.2;
            height: 100%;
            width: 100%;
            /* overflow: hidden; */
        }

        #Enroll #formgr h2 {
            margin: 7px;
            padding: 5px;
            font-size: 2rem;
            font-family: 'Merienda One', cursive;
            text-align: center;
        }

        #Enroll #formgr form label {
            margin: 7px;
            padding: 5px;
            font-size: 1.2rem;
            color: black;
            font-weight: bolder;
            font-family: 'Noto Serif', serif;
            overflow: hidden;
            cursor: pointer;
        }

        #Enroll #formgr form #btn {
            margin: 7px;
            padding: 5px;
            font-size: 1rem;
            border-radius: 5px;
            background: black;
            color: white;
            font-weight: bolder;
            font-family: 'Noto Serif', serif;
            cursor: pointer;
        }

        #Enroll #formgr form input,
        #Enroll #formgr form textarea {
            border-radius: 5px;
            overflow: hidden;
            cursor: pointer;
        }
        @media only screen and (max-width: 1100px)
        {
            #Courses{
                margin-top: 400px;
            }
        }
        @media only screen and (max-width: 777px) {
            #navbars {
                flex-direction: column;
                align-items: center;
                justify-content: center;
                padding: 0px;
            }

            #navbars img {
                height: 60px;
                width: 75px;
            }

            #navbars ul {
                margin: 2px 2px;
            }

            #navbars ul li {
                margin: 2px 5px;
                align-items: center;
                justify-content: center;
            }

            #navbars ul li a {
                font-size: 14px;
            }

            #Home #head {
                margin: 2px 0px;
                padding: 0px;
            }

            #Home ::before {
                height: 60%;
            }

            #Home #head h1 {
                margin: 0px;
                padding: 0px;
                font-size: 26px;
                text-align: center;
            }

            #Home #head p {
                margin: 0px;
                padding: 0px;
                font-size: 14px;
                text-align: center;
            }

            #Courses {
                margin-top: 400px;
                width: 100%;
                height: auto;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                flex-wrap: wrap;
            }

            #Courses #course {
                margin: 31px 0px;
                padding: 15px 0px;
            }

            #Courses #course h2 {
                margin: 5px 0px;
                padding: 3px 0px;
                font-size: 26px;
            }

            #Courses #course #subject {
                flex-direction: column;
            }

            #Courses #course #subject .subjects {
                margin: 5px 15px;
                /* overflow: hidden; */
            }

            #Courses #course #subject .subjects img {
                margin: 2px;
                height: 70px;
                width: 75px;
            }

            #Courses #course #subject .subjects h3 {
                margin: 0px 2px;
                padding: 2px;
                text-align: center;
                font-size: 20px;
            }

            #Courses #course #subject .subjects p {
                margin: 4px 0px;
                padding: 6px 0px;
                text-align: center;
                font-size: 13px;
            }

            #Faculties div h2 {
                margin: 7px 0px;
                padding: 0px;
                font-size: 20px;
            }

            #Faculties div p {
                margin: 4px 0px;
                padding: 5px;
                font-size: 13px;
            }

            #Enroll #formgr h2 {
                margin: 6px 0px;
                padding: 0px;
                font-size: 20px;
            }

            #Enroll #formgr form label {
                margin: 2px 0px;
                padding: 1px;
                font-size: 12px;
            }

            #Enroll #formgr form #btn {
                margin: 4px 0px;
                padding: 1px;
                font-size: 11px;
            }
        }
        /* Pseudo selectors */
        #navbars ul li :hover{
            background-color: rgb(119, 15, 167);
            border-radius: 5px;
            color: black;
            text-decoration: underline;
        }
        #navbars ul li :active{
            background-color: red;
            border-radius: 5px;
            color: black;
            text-decoration: underline;
        }
    </style>
</head>

<body>
    <nav id="navbars">
        <img src="https://cdn.pixabay.com/photo/2017/02/13/08/54/brain-2062057_960_720.jpg" alt="Our logo" id="logo">
        <ul>
            <li><a href="#Home">Home</a></li>
            <li><a href="#Courses">Courses offered</a></li>
            <li><a href="#Faculties">About Faculties</a></li>
            <li><a href="#Enroll">Enroll</a></li>
        </ul>
    </nav>
    <section id="Home">
        <div id="head">
            <h1>Welcome to Our online courses</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate rerum vel perspiciatis voluptatem
                officia ab, rem similique id. Maiores, pariatur.</p>
        </div>
    </section>
    <section id="Courses">
        <div id="course">
            <h2>Our Courses</h2>
            <div id="subject">
                <div class="subjects" id="physics">
                    <img src="https://cdn.pixabay.com/photo/2015/11/15/07/47/geometry-1044090_960_720.jpg" alt="">
                    <h3>About our physics course</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis odit possimus numquam qui
                        doloremque excepturi nulla. Similique sed enim temporibus facilis obcaecati quam et vel ut
                        minus!
                        Delectus perferendis neque totam voluptatum sequi quam magnam error illum, enim numquam
                        voluptate?</p>
                </div>
                <div class="subjects" id="chemistry">
                    <img src="https://cdn.pixabay.com/photo/2015/04/26/13/47/chemistry-740453_960_720.jpg" alt="">
                    <h3>About our chemistry course</h3>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Perspiciatis voluptatem voluptatum
                        doloribus
                        delectus adipisci debitis officia quos repellendus fuga quis vitae voluptates, molestias atque,
                        animi
                        nobis voluptate. Accusantium reprehenderit, earum nemo odio ad quia rem? Dolores exercitationem
                        aperiam
                        cumque saepe.</p>
                </div>
                <div class="subjects" id="maths">
                    <img src="https://cdn.pixabay.com/photo/2015/05/08/05/09/mathematics-757566_960_720.jpg" alt="">
                    <h3>About our mathematics course</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, perspiciatis doloribus. Autem,
                        facilis
                        vero. Dignissimos possimus obcaecati aliquam quam corporis numquam nemo necessitatibus similique
                        a
                        excepturi illo sunt veritatis culpa laborum commodi consequatur nobis, magni blanditiis tenetur
                        alias?
                        Impedit, quis!</p>
                </div>
            </div>
        </div>
    </section> 
    <section id="Faculties">
        <div>
            <h2>About our Faculties</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, reiciendis harum eius eaque quidem vero.
                Similique est veniam voluptatum pariatur magnam assumenda totam perspiciatis et veritatis aliquid
                voluptate modi atque ratione, perferendis eligendi dolorem esse inventore omnis rerum corporis fuga quos
                quia fugit. Odio, dignissimos suscipit! Provident iste repellat animi eligendi iusto! Omnis est
                accusantium recusandae sunt quisquam vero harum iste, sed libero aliquam ducimus accusamus molestias
                cupiditate incidunt eos nemo excepturi dolore! Vel repellat incidunt sunt explicabo. Soluta perspiciatis
                quidem reprehenderit at qui tenetur blanditiis debitis non, ipsum enim facere quasi. Commodi inventore
                magnam libero nam blanditiis laudantium possimus ad obcaecati eius fugiat reiciendis sit, tenetur amet
                quia perferendis cumque ullam doloribus maiores consequatur cupiditate voluptas laboriosam! Veritatis
                tenetur itaque deserunt recusandae dignissimos explicabo sapiente quasi quas porro pariatur cumque,
                blanditiis saepe delectus? Neque quis quibusdam itaque tenetur, molestiae eveniet quia hic! Voluptates,
                ullam! Esse omnis quos aliquid id, nobis repudiandae illo voluptatem minima dolores hic. Et molestiae
                iste soluta blanditiis eligendi consequuntur, alias esse, fugiat maiores praesentium, laboriosam eveniet
                sed asperiores officia iusto error quam doloremque ex. Aperiam voluptates, modi, voluptas perspiciatis
                culpa distinctio in a dolores cumque explicabo quo, molestiae reprehenderit perferendis voluptatem!
                Voluptate quidem consequatur quia.</p>
        </div>
    </section>
    <section id="Enroll">
        <div id="formgr">
            <h2>Fill up this form to Enroll</h2>
            <form action="">
                <label for="name">Name: </label>
                <input type="text" id="name" placeholder="Enter your name here">
                <label for="email">Email Id: </label>
                <input type="email" id="email" placeholder="Enter your email Id">
                <label for="dob">Date of Birth</label>
                <input type="date" id="dob" placeholder="Date of Birth">
                <label for="phno.">Phone number: </label>
                <input type="number" id="phno." placeholder="Enter your number here">
                <label for="addr">Address: </label>
                <input type="text" id="addr" placeholder="Enter your address">
                <label for="aboutyou">About yourself: </label>
                <textarea name="" id="aboutyou" cols="10" rows="10"></textarea>
                <button id="btn">Submit</button>
            </form>
        </div>
    </section>
</body>

</html>
