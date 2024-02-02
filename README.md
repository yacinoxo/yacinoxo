skills css like solar system : 

@tailwind base;
@tailwind components;
@tailwind utilities;


.Skills-section{
    margin: 0;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: black;
    overflow: hidden;
}
.container {
    font-size: 12px;
    width: 80em;
    height: 80em;
    position: relative;
    scale: 0.4;
}

.sun {
    display: flex;
    align-items: center;
    justify-content: center;
    position: absolute;
    top: 30em;
    left: 30em;
    width: 20em;
    height: 20em;
    border-radius: 50%;
    box-shadow: 0 0 6em rgb(255, 128, 0);
    animation: orbit 50s linear infinite;
}

.earth,
.moon,
.saturn,
.neptune,
.tailwind {
    position: absolute;
    border-style: solid;
    border-color: white transparent transparent transparent;
    border-width: 0.2em 0.2em 0 0;
    border-radius: 50%;
}


.earth {
    top: 12em;
    left: 12em;
    width: 56em;
    height: 56em; 
    animation: orbit 36.5s linear infinite;   
}
.moon {
    top: 4em;
    right: -2em;
    width: 14em;
    height: 14em; 
    animation: orbit 2.7s linear infinite;
}

.tailwind {
    top: 9em;
    right: 5em;
    width: 28em;
    height: 28em; 
    animation: orbit 2.7s linear infinite;
}

.saturn {
    top: -14em;
    left: -14em;
    width: 110em;
    height: 110em; 
    animation: orbit 17s linear infinite;
}

.neptune {
    top: -34em;
    left: -34em;
    width: 150em;
    height: 150em; 
    animation: orbit 36.5s linear infinite;
}


.earth::before,
.moon::before,
.tailwind::before,
.saturn::before,
.neptune::before{
    content: '';
    position: absolute;
    border-radius: 50%;
    animation: orbit 30s linear infinite;
}

.earth::before {
    top: 6em;
    right: 0em;
    width: 10em;
    height: 10em;
    background-image: url("https://miro.medium.com/v2/resize:fit:800/1*v2vdfKqD4MtmTSgNP0o5cg.png");
    background-size: cover;
}

.moon::before {
    top: 1.6em;
    right: 0.4em;
    width: 2.4em;
    height: 2.4em;
    background-image: url("https://www.drupal.org/files/project-images/nextjs-icon-dark-background.png");
    background-size: cover;
}

.tailwind::before {
    top: 4em;
    right: .6em;
    width: 5em;
    height: 5em;
    background-image: url("https://codekitapp.com/images/help/free-tailwind-icon@2x.png");
    background-size: cover;
}

.saturn::before {
    top: 15em;
    right: 10em;
    width: 9em;
    height: 9em;
    background-image: url("https://cdn.icon-icons.com/icons2/2107/PNG/512/file_type_html_icon_130541.png");
    background-size: cover;
}

.neptune::before {
    top: 20em;
    right: 16em;
    width: 8em;
    height: 8em;
    background-image: url("https://diziglobalsolution.com/wp-content/uploads/2023/04/logo-css-3-1536.png");
    background-size: cover;
}


@keyframes orbit {
    to {
        transform: rotate(360deg);
    }
}
