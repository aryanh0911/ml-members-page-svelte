<script>
    export let memberImg, memberName, memberRole, githubLink, linkedInLink, facebookLink;

</script>




<div class="card">
    <div class="member-image">
        <img src={memberImg} alt="">
    </div>

    <div class="member-name">
        <p>{memberName}</p>
    </div>

    <div class="member-role">
        <p>{memberRole}</p>
    </div>

    <div class="member-contacts">
        <div>
            <!-- GITHUB -->
            <a href={githubLink}><i class="ri-github-fill"></i></a>
            
            <!-- LINKEDIN -->
            <a href={linkedInLink} style="text-decoration: none; color: #b8b8b8"><i class="ri-linkedin-box-fill"></i></a>
            
            <!-- FACEBOOK -->
            <a href={facebookLink} style="text-decoration: none; color: #b8b8b8"><i class="ri-facebook-circle-fill"></i></a>


        </div>
    </div>
</div>





<!-- STYLES -->
<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');  

    .card {
        background-color: rgba(0, 0, 0, 0.596);
        box-sizing: border-box;
        margin: 0 auto;
        /* padding: 3rem 1rem; */
        color: rgba(255, 255, 255, 0.863);
        border: 1px solid rgb(0, 0, 0);
        border-radius: 1.3rem;
        /* padding: 1rem; */
        max-width: 360px;
        min-width: 250px;
        backdrop-filter: blur(1.5px);
        box-shadow: 0 8px 8px rgba(0, 0, 0, 0.546);
        transition: backdrop-filter 0.2s, transform .3s, box-shadow .3s;
    }

    .member-image {
        padding-top: 3rem;
        padding-bottom: 1rem;
    }

    .member-image img {
        border-radius: 50%;
        width: 11rem;
        height: 11rem;
        /* object-fit: cover; */;
        border: 3px solid #ff7801;
        padding: .2rem;
        /* margin-bottom: 20rem; */
    }

    .member-name {
        font-family: Montserrat,sans-serif;
        font-size: 1.3rem;
        font-weight: 700;
        /* font-size: .9rem; */
    }

    .member-role {
        font-weight: 200;
        font-size: 1.2rem;
        margin-top: .2rem;
    }

    .member-contacts div {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: .8rem;
    }

    .member-contacts {
        margin-top: 1.8rem;
        margin-bottom: 2.3rem;
        font-size: 1.5rem;
        color: red;
    }

    .member-contacts a {
        text-decoration: none; 
        color: #b8b8b8;
        cursor: pointer;
    }

    .card:hover {
        backdrop-filter: blur(8px);
        transform: translateY(-4px);
        box-shadow: 4px 12px 9px rgba(0, 0, 0, 0.546);
    }
    
</style>