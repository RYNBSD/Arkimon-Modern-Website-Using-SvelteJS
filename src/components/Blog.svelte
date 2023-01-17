<script>
    import Fa from "svelte-fa";
    import { faArrowRight } from "@fortawesome/free-solid-svg-icons";

    import { blogData } from "../constants";
</script>

<section class="arkimon__blog" id="news">
    <div class="arkimon__blog-container f-center">
        <div class="arkimon__blog-container_top f-center">
            <h1>Early Digital Explorations From Our Daily Blog</h1>
            <button type="button">
                Read Our Blog
                <Fa icon={faArrowRight} />
            </button>
        </div>
        <div class="arkimon__blog-container_bottom">
            {#each blogData as blog, index (index)}
                <div
                    class="arkimon__blog-container_bottom-img"
                    style={`background-image: url('${blog}');`}
                    role="banner"
                >
                    <div class="arkimon__blog-container_bottom-img_content f-center">
                        <p>by <span>Monju Aflame</span>, 3 days ago</p>
                        <h2>Beef Meat sit amet, cte tur adipiscing....</h2>
                        <Fa icon={faArrowRight} size="3x" primaryColor="#fff" />
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>