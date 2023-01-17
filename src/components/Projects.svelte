<script>
    import Fa from 'svelte-fa';
    import { faArrowLeft, faArrowRight } from '@fortawesome/free-solid-svg-icons';


    import { projects1, projects2, projects3 } from '../constants';

    const images = [projects1, projects2, projects3];

</script>

<section class="arkimon__projects" id="projects">
    <div class="arkimon__projects-container f-center">
        <div class="arkimon__projects-container_info f-center">
            <h1>Amazing projects from most talented builders architects & designers</h1>
            <div class="arkimon__projects-container_info-arrows f-center">
                <Fa icon={faArrowLeft} primaryColor="#4E4E4E" size="4x" />
                <Fa icon={faArrowRight} primaryColor="#FDAE54" size="4x" />
            </div>
        </div>
        <div class="arkimon__projects-container-images">
            {#each images as image, index (index)}
                <img src={image} alt="images">
            {/each}
        </div>
    </div>
</section>