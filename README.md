# Frontend Mentor - NFT preview card component

![Design preview for the NFT preview card component coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Thanks for reading this front-end coding challenge solution.

[Frontend Mentor](https://www.frontendmentor.io) challenges help you improve your coding skills by building realistic projects.

##### Ce que j'ai retenu 

# Centrer le body 

body 
{ 
display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    min-height: 100vh;
}

# Préférable d'utiliser margin 0 auto au lieu de display flex (ce qui est en haut)
.boite {
    margin: 0 auto;
}
# Pour les margin utiliser du rem car cela s'adapte au zoom de l'écran 

.contenu {
    margin: 2rem 1rem;
}

# NE pas oublier comment mettre une image sur une image avec un background au surf 

.imagedebut {
    border-radius: 12px;
    overflow: hidden;
    position: relative;
}
.imagedebut img {
    width: 100%;
    display: block;
}
.overlay {
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0;
    display: none;
    background-color: hsla(178, 100%, 50%,0.5);
}
.overlay img {
    position: absolute;
    left: 50%;
    top: 50%;
    width: 50px;
    transform: translate(-50%,-50%);
}
.imagedebut:hover .overlay {
    display: block;
}
# NE pas hésiter à utilser 

display: inline-block;