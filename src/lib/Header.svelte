<script>

let menu = document.querySelector('#menu-icon');
let navbar = document.querySelector('.navbar');

/*menu.onclick = () => {
    menu.classList.toggle('bx-x');
    navbar.classList.toggle('open');
}*/

/*menu.addEventListener('click', ()=>{
    menu.classList.toggle('bx-x');
    navbar.classList.toggle('open');
});*/

</script>

<main>

    <header>
        <a href="" class="logo"><i class="ri-book-mark-fill"></i><span>Read me! Now!</span></a>
        <ul class="navbar">
            <li><a href="#" class="activate"> Home </a></li>
            <li><a href="#"> About Us </a></li>
            <li><a href="#"> Services </a></li>
            <li><a href="#"> Blog </a></li>
            <li><a href="#"> Contact </a></li>
        </ul>
    
        <div class="main">
            <a href="#" class="user"><i class="ri-user-fill"></i>Sign In</a>
            <a href="#">Register</a>
            <div class="bx bx-menu" id="menu-icon" ></div>
        </div>
    </header>

</main>



<style>

header{
    position: fixed;
    width: 100%;
    top: 0;
    right: 0;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: white;
    padding: 28px 12% ;
    transition: all .50s ease;
}

.logo{
    display: flex;
    align-items: center;
}

.logo i{
    color: #3b285b;
    font-size: 28px;
    margin-right: 3px;
}

.logo span{
    color: #745ba3;
    font-size: 1.7rem;
    font-weight: 600;
}

.navbar{
    display: flex;
}

.navbar a{
    color: #745ba3;
    font-size: 1.1rem;
    font-weight: 500;
    padding: 5px 0;
    margin: 0px 30px;
    transition: all .50s ease;
}

.navbar a:hover{
    color: #3b285b;
}

.navbar a.activate{
    color: #3b285b;
}

.main{
    display: flex;
    align-items: center;
}

.main a{
    margin-right: 25px;
    margin-left: 10px;
    color: #745ba3;
    font-size: 1.1rem;
    font-weight: 500;
    transition: all .50s ease;
}

.user{
    display: flex;
    align-items: center;
}

.user i{
    color: #3b285b;
    font-size: 28px;
    margin-right: 7px;
}

.main a:hover{
    color: #3b285b;
}

#menu-icon{
    font-size: 35px;
    color: #745ba3;
    cursor: pointer;
    z-index: 10001;
    display: none;
}

@media (max-width: 1280px){
    header{
        padding: 14px 2%;
        transition: .2s;
    }

    .navbar a{
        padding: 5px 0;
        margin: 0px 20px;
    }
}

@media (max-width: 1090px){
    #menu-icon{
        display: block;
    }

    .navbar{
        position: absolute;
        top: 100%;
        right: -100%;
        width: 270px;
        height: 34vh;
        background: #3b285b;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        border-radius: 10px;
        transition: all .50s ease;
    }

    .navbar a{
        display: block;
        margin: 12px 0;
        padding: 0px 25px;
        transition: all .50s ease;
    }

    .navbar a:hover{
        color: #745ba3;
        transform: translateY(5px);
    }

    .navbar a.activate{
        color: #745ba3;
    }

    .navbar.open{
        right: 2%;
    }
}
</style>