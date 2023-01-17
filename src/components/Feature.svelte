<script>
    import Fa from "svelte-fa";
    import { faArrowRight } from '@fortawesome/free-solid-svg-icons';

    import { featureData } from "../constants";
</script>

<section class="arkimon__feature">
    
    <div class="arkimon__feature-container">
        {#each featureData as feature (feature.title)}
            <div class="arkimon__feature-container_element f-center">
                <div class="arkimon__feature-container_element-icon">
                    <Fa icon={feature.icon} size="3x" />
                </div>
                <div class="arkimon__feature-container_element-title">
                    <h1>{feature.title}</h1>
                </div>
                <div class="arkimon__feature-container_element-desc">
                    <p>Morbi volutpat nisi a ligula vestibulum placerat. Suspendisse venenatis pulvinar nibh sed convallis</p>
                </div>
                <div class="arkimon__feature-container_element-arrow">
                    <Fa icon={faArrowRight} size="3x" primaryColor="#FDAE54" />
                </div>
            </div>
        {/each}
    </div>
</section>