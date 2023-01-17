<script>
    import { servicesData, services } from "../constants";
</script>

<section class="arkimon__services" id="services">
    <div class="arkimon__services-container">
        <div class="arkimon__services-container_left">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src={services} alt="image" />
        </div>
        <div class="arkimon__services-container_right f-center">
            <h1>We are designing amazing staff from last 5 years</h1>
            <div class="arkimon__services-container_right-elements">
                {#each servicesData as service, index (service)}
                    <div class="arkimon__services-container_right-elements_element f-center">
                        <div class="arkimon__services-container_right-elements_element-index">
                            <h2>0{index+1}/</h2>
                        </div>
                        <div class="arkimon__services-container_right-elements_element-content">
                            <h2>{service}</h2>
                        </div>
                    </div>
                {/each}
            </div>
        </div>
    </div>
</section>