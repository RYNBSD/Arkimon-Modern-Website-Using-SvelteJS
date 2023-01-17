<script>
    import Fa from 'svelte-fa';
    import { faBuilding } from '@fortawesome/free-solid-svg-icons';

    import { experienceData } from '../constants';
</script>

<section class="arkimon__experience">
    <div class="arkimon__experience-container f-center">
        <div class="arkimon__experience-container_title f-center">
            <div class="dash" />
            <h1>We Create Digital Experience Local To Worldwide</h1>
            <div class="buble1" />
            <div class="buble2" />
        </div>
        <div class="arkimon__experience-container_elements">
            {#each experienceData as experience (experience)}
                <div class="arkimon__experience-container_elements-element f-center">
                    <Fa icon={faBuilding} size="3x" />
                    <h2>{experience}</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare sit convallis risus sit elit. Rutrum arcu cursus aenean ut.</p>
                </div>
            {/each}
        </div>
    </div>
</section>