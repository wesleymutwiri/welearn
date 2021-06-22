<script>
    import SmallCard from "../components/SmallCard.svelte"
    import Box from "../components/Box.svelte"
</script>
<div class="container">
    <div class="row">
        <div class="column">
            <h3>Hi Wesley,</h3>
            <h1>What will you learn today?</h1>
            <div class="carousel-box">
                <div class="carousel-image">
                    <img src="notifications.svg" alt="">
                </div>
                <div class="carousel-text">
                    <h3>Artificial Intelligence for Marketing</h3>
                    <p>Learn how artificial intelligence is reshaping the way marketing is done at both large and small
                        organizations</p>
                    <button class="learn-now">Learn Now</button>
                </div>
            </div>
            <h3>Your learning path</h3>
            <div class="row">
                <Box />
                <Box />
                <Box />

            </div>
        </div>
        <div class="column">
            <div class="row nav">
                <div class="search-input">
                    <input type="search" name="search" id="" placeholder="Search">
                    <svg viewBox="0 0 24 24" width="24" height="24" stroke="currentColor" stroke-width="2" fill="none"
                        stroke-linecap="round" stroke-linejoin="round" class="css-i6dzq1">
                        <circle cx="11" cy="11" r="8"></circle>
                        <line x1="21" y1="21" x2="16.65" y2="16.65"></line>
                    </svg>
                </div>
                <div class="notification">
                    <svg viewBox="0 0 24 24" width="24" height="24" stroke="currentColor" stroke-width="2" fill="none"
                        stroke-linecap="round" stroke-linejoin="round" class="css-i6dzq1">
                        <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                        <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
                    </svg>
                </div>
            </div>
            <div class="courses">
                <h4>Course in Progress</h4>
                <div class="column">
                    <SmallCard />
                    <SmallCard />
                    <SmallCard />
                    <SmallCard />
                </div>
            </div>
            <div>
                <div class="column">
                    <h4>Your learning point</h4>

                </div>
            </div>
        </div>
    </div>
</div>

<style>
    .container {
        padding: 0 2rem;
    }

    .column {
        font-family: 'Poppins', sans-serif;
        width: 50%;
        padding: 0 1rem;
    }

    .search-input {
        position: relative;
        padding: 0.5rem 1rem;
        vertical-align: middle;
        white-space: nowrap;
        display: flex;
        align-items: center;
    }

    .search-input input {
        border: none;
        padding-left: 1.5rem;
        outline: none;
    }

    .search-input svg {
        position: absolute;
        left: 0;
    }

    .carousel-box {
        background: #3f8cff;
        width: 100%;
        height: 400px;
        border-radius: 1rem;
        box-shadow: 0px 10px 0 -3px #3f8cff70, 0px 20px 0 -7px #3f8cff48;
        display: flex;
        padding: 1rem;
        margin-bottom: 6rem;
    }

    .carousel-image img {
        height: 100%;
        width: 60%;
    }

    .carousel-text {
        color: #fff;
        margin: auto;
        /* width: 200px; */
        line-height: 1.5;
        /* display: flex;
        flex-direction: column;
        justify-content: space-between; */
    }

    .carousel-text p {
        font-weight: lighter;
    }

    .carousel-text h3 {
        font-weight: 600;
        font-size: 1.5rem;
    }

    .learn-now {
        border: none;
        background: #fdfdfd;
        color: #2d2d2f;
        padding: 1rem 2rem;
        border-radius: 1rem;
    }

    h1,
    h3 {
        font-weight: 300;
    }

    .notification {
        background: #fff;
        padding: 1rem;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .text-light {
        color: #808191;
    }

    .courses {
        margin: 2rem 0;
    }
    h1, .nav {
        margin-bottom: 3rem;
    }
</style>