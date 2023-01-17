<script>
    import Fa from 'svelte-fa';
    import { faArrowLeft, faArrowRight, faThumbsUp } from '@fortawesome/free-solid-svg-icons';


    import { testimonial } from "../constants";
</script>

<section class="arkimon__testimonial">
    <div class="arkimon__testimonial-container">
        <div class="arkimon__testimonial-container_left">
            <img src={testimonial} alt="testimonial">
        </div>
        <div class="arkimon__testimonial-container_right f-center">
            <div class="arkimon__testimonial-container_right-arrows f-center">
                <Fa icon={faArrowLeft} primaryColor="#4E4E4E" size="4x" />
                <Fa icon={faArrowRight} primaryColor="#FDAE54" size="4x" />
            </div>
            <h1>I am ipsum dolor sit amet, consectetur adipiscing elit. Ornare sit convallis risus sit elit. Rutrum arcu cursus aenean ut.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare sit convallis </h1>
            <div class="arkimon__testimonial-container_right-author f-center">
                <div class="arkimon__testimonial-container_right-author_name f-center">
                    <Fa icon={faThumbsUp} size="2x" primaryColor="#FDAE54" />
                    <h3>Shahid Zaman</h3>
                </div>
                <div class="arkimon__testimonial-container_right-author_skills">
                    <small>Graphic Designer, Intelligent Project</small>
                </div>
            </div>
        </div>
    </div>
</section>