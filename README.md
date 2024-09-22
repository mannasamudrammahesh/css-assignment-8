<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animal Blog</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f7e4c3;
        }
        h1 {
            text-align: center;
            margin-top: 20px;
        }
        .main-grid {
            display: grid;
            grid-template-areas: 
                "header header header"
                "sidebar content content"
                "footer footer footer";
            grid-template-rows: 100px 1fr 50px;
            grid-template-columns: 250px 300px 1fr;
            gap: 10px;
            padding: 10px;
        }
        .header {
            grid-area: header;
            background-color: #c8a97e;
            padding: 10px;
            color: white;
            text-align: center;
            font-size: 1.5em;
            position: relative;
        }
        .nav {
            position: absolute;
            top: 10px;
            right: 10px;
        }
        .nav a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
            font-weight: bold;
        }
        .nav a:hover {
            text-decoration: underline;
        }
        .sidebar {
            grid-area: sidebar;
            background-color: #d5bda5;
            padding: 10px;
            height: 98.75%;
        }
        .sidebar h2 {
            margin-top: 0;
        }
        .category-item {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
            padding: 10px;
            background-color: #e4d3c1;
            border-radius: 5px;
        }

        .category-item img {
            width: 50px;
            height: 50px;
            margin-right: 10px;
            border-radius: 50%;
            cursor:pointer;
        }

        .content {
            grid-area: content;
            display: grid;
            grid-template-areas:
                "main aside"
                "main aside";
            grid-template-rows: 1fr 1fr;
            grid-template-columns: 1.5fr 1fr;
            gap: 10px;
            background-color: #e4d3c1;
            padding: 10px;
        }

        .main-content {
            grid-area: main;
            background-color: #f7f0eb;
            padding: 10px;
        }

        .aside {
            grid-area: aside;
            background-color: #f4e9e1;
            padding: 10px;
        }
        .footer {
            grid-area: footer;
            background-color: #c8a97e;
            padding: 10px;
            color: white;
            text-align: center;
        }
        .call-to-action {
            background-color: #d5bda5;
            padding: 20px;
            text-align: center;
            margin-top: 10px;
            border-radius: 5px;
        }

        .call-to-action h2 {
            margin: 0;
        }
        .call-to-action p {
            margin: 10px 0;
        }
        .call-to-action button {
            background-color: #c8a97e;
            border: none;
            color: white;
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
        }
        .call-to-action button:hover {
            background-color: #b89a6f;
        }
        .social-media {
            margin: 10px 0;
            text-align: center;
        }
        .social-media a {
            text-decoration: none;
            color: #c8a97e;
            margin: 0 10px;
            font-size: 1.2em;
        }
        .social-media a:hover {
            color: #a67f5d;
        }
        .grid-item {
            border: 2px solid #ccc;
            border-radius: 5px;
            overflow: hidden;
            padding: 10px;
            background-color: #ffffff;
            cursor:pointer;
        }
        .grid-item img {
            width: 100%;
            height: auto;
            display: block;
        }
        .news-item img{
width:130px;
height:120px;
cursor:pointer;
}
    </style>
</head>
<body>
    <div class="main-grid">
        <div class="header">
            <h1>Animal Blog</h1>
            <div class="nav">
                <a href="#">Home</a>
                <a href="#">About</a>
                <a href="#">Contact</a>
            </div>
        </div>
        <div class="sidebar">
            <h2>Categories</h2>
            <div class="category-item">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%3Fid%3DOIP.vL4-z2iMTtquIWCPfuRelQHaI2%26pid%3DApi&f=1&ipt=9583a4918e608d9ce85b1c0c8e8d959dcdbdafc3fd4d10ddc71038f5f1400770&ipo=images" alt="Mammals">
                <div>
                    <h3>Mammals</h3>
                    <p>Explore the diverse world of mammals, from majestic lions to playful dolphins.</p>
                </div>
            </div>
            <div class="category-item">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.SH3M_VSuujbbMN5mLyXqMAHaE9%26pid%3DApi&f=1&ipt=06d62b366b744de68ad11f09690c11be777b6d408cf914f855037b7a56d6c229&ipo=images" alt="Birds">
                <div>
                    <h3>Birds</h3>
                    <p>Discover the fascinating lives of birds, including their unique behaviors and habitats.</p>
                </div>
            </div>
            <div class="category-item">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%3Fid%3DOIP.weJZCT0ZleoQLChxuWWWTAHaE7%26pid%3DApi&f=1&ipt=d2201e681551cf221ad1deac73157c7b0d97417d1910cfc8206630821638b086&ipo=images" alt="Reptiles">
                <div>
                    <h3>Reptiles</h3>
                    <p>Learn about reptiles, from colorful chameleons to fearsome crocodiles.</p>
                </div>
            </div>
            <div class="category-item">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.dikeVJRMsNAY9bcrcxHRfQHaEK%26pid%3DApi&f=1&ipt=3e171e64ccc96cb0acddb978b3548281a53a378992cc0ac0ccde94510efa4b74&ipo=images" alt="Amphibians">
                <div>
                    <h3>Amphibians</h3>
                    <p>Explore the intriguing world of amphibians, including frogs, toads, and salamanders.</p>
                </div>
            </div>
            <div class="category-item">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%3Fid%3DOIP.SimzT9Q_o9_bsEFh5PWcOAHaEo%26pid%3DApi&f=1&ipt=311ececce2cc9b30925dc9b20ca08f044ce05632c8b08b8b9be099086a963400&ipo=images" alt="Fish">
                <div>
                    <h3>Fish</h3>
                    <p>Dive into the aquatic world of fish, from vibrant coral reef species to deep-sea wonders.</p>
                </div>
            </div>
        </div>
        <div class="content">
            <div class="main-content">
                <h2>Featured Articles</h2>
                <div class="grid-item">
                    <img src="https://media.istockphoto.com/id/663981890/photo/zebra-at-sunset-in-the-serengeti-national-park-africa-tanzania.jpg?s=612x612&w=0&k=20&c=oq2K_SwrG6tvyFAkMDTVV5CmnQygibxpRCvxb3apwdE=" alt="Zebra">
                    <h3>Zebras in the Serengeti</h3>
                    <p>Discover the majestic beauty of zebras in their natural habitat. The Serengeti offers a unique experience for wildlife enthusiasts.</p>
                </div>
                <div class="grid-item">
                    <img src="https://media.istockphoto.com/id/1489566726/photo/leopard-in-sri-lanka.jpg?s=612x612&w=0&k=20&c=kIHqKhwO_JCq94l7yg8zkZuY-v-BbiaaRxr-giy97w4=" alt="Leopard">
                    <h3>Leopards of Sri Lanka</h3>
                    <p>Explore the elusive leopards of Sri Lanka. Learn about their habitat, behavior, and conservation efforts.</p>
                </div>
                <div class="grid-item">
                    <img src="https://media.istockphoto.com/id/501965551/photo/picture-presenting-the-galloping-white-horse.jpg?s=612x612&w=0&k=20&c=hxVH5rpHUBJ6_pnRzQR1bI_cfiivl9-W8G-FhNKfmio=" alt="White Horse">
                    <h3>Galloping White Horses</h3>
                    <p>The white horses of the Camargue region are a sight to behold. Their grace and strength are unmatched.</p>
                </div>
            </div>
            <div class="aside">
                <h2>Latest News</h2>
                <div class="news-item">
                    <img src="https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fi.huffpost.com%2Fgen%2F3099178%2Fimages%2Fo-RHINOCEROS-facebook.jpg&f=1&nofb=1&ipt=90e6468dcc1b1a938d80b667df228f11cd7eb7476b3094890bd0f7a9493e8258&ipo=images" alt="Rhino Conservation">
                    <h3>New Rhino Conservation Efforts</h3>
                    <p>Recent advancements in rhino conservation aim to protect these majestic creatures from poaching and habitat loss.</p>
<p>Rhinoceroses, often simply called “rhinos,” are amongst the largest of all land animals on the Earth. Because of this, they are often classified as “megafauna,” which refers to animals over 2,200 lb (1,000 kg). The name “rhinoceros” comes from the Greek “rhino” (nose) and “ceros” (horn), because all 5 species of rhino have either 1 or 2 horns on their nose. </p>
                </div>
                <div class="news-item">
<h3>Rare Birds </h3>
                    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.5dGImwmpmE5Ej-H3URmq2AAAAA%26pid%3DApi&f=1&ipt=7052475f4ed67a1def6a5f661313a0c63317bea8c863b4c143f5bb81682ad137&ipo=images" alt="Rare Birds></div>
<h3>Philippine Eagle </h3>
<img src="https://a-z-animals.com/media/2021/05/Largest-Eagles-in-the-World_-Philippine-Eagle-1024x535.jpg" alt="Philippine Eagle">
<p>This bird is native to the Philippines, where it is the country’s national bird. The Philippine eagle is critically endangered, however, and experts estimate that fewer than 500 remain.
These rare birds are among the world’s largest species of eagles. They can reach heights of 3 feet with wingspans of 6.5 feet. Philippine eagles can be recognized by their distinctive brown and white crest, which circles their heads like a mane.  </p>
</div>
</div>
</body>
</html>
