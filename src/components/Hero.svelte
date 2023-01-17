<script>
    import Fa from 'svelte-fa';
    import { faArrowRight } from '@fortawesome/free-solid-svg-icons';

    import Navbar from './Navbar.svelte';
    import { hero } from '../constants';
</script>

<header id="home" class="arkimon__hero">
    <Navbar />
    <div class="arkimon__hero-container">
        <div style="display: flex; width: 100%; height: 100%;" class="f-center">
            <div class="arkimon__hero-container_left f-center">
                <h1>Elegant Interior Design for your home & office</h1>
                <p>Cras vel cursus libero. Vestibulum porttitor nunc enim, quis congue leo fringilla ut. Quisque in lacus lacus. Nunc malesuada.</p>
                <button type="button" class="f-center">
                    Explore Projects
                    <Fa icon={faArrowRight} />
                </button>
            </div>
        </div>
        <div class="arkimon__hero-container_right">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src={hero} alt="image" />
        </div>
    </div>
</header>