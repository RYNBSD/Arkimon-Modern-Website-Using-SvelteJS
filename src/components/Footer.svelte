<script>
    import Fa from "svelte-fa";

    import { logoDark } from "../constants";
</script>

<footer class="arkimon__footer">
    <div class="arkimon__footer-container f-center">
        <div class="arkimon__footer-container_top">
            <ul>
                <li>
                    <h1>Company</h1>
                </li>
                <li>Career</li>
                <li>About Us</li>
                <li>Blog</li>
                <li>Feature</li>
                <li>Story</li>
            </ul>
            <ul>
                <li>
                    <h1>Design</h1>
                </li>
                <li>2D Designer</li>
                <li>3D Designer</li>
                <li>Collaboration</li>
                <li>Tools</li>
                <li>Important Link</li>
            </ul>
            <ul>
                <li>
                    <h1>Links</h1>
                </li>
                <li>Projects</li>
                <li>Contact</li>
                <li>Send Email</li>
                <li>Fiver</li>
                <li>upWork</li>
            </ul>
            <ul>
                <li>
                    <h1>Material</h1>
                </li>
                <li>Company Profile</li>
                <li>Asset</li>
                <li>Location Map</li>
                <li>Estimate Cost</li>
                <li>Default Quotation</li>
            </ul>
            <ul class="arkimon__footer-container_top-contact">
                <li>
                    <h1>Subscribe</h1>
                </li>
                <li>
                    <input type="text">
                </li>
                <li>
                    <input type="button" value="Subscribe" placeholder="Email Address">
                </li>
            </ul>
        </div>
        <div class="arkimon__footer-container_split" />
        <div class="arkimon__footer-container_bottom">
            <img src={logoDark} alt="logo">
        </div>
    </div>
</footer>