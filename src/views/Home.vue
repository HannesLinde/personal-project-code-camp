<template>
  <div>
    <!-- START HEADER -->
    <header>
      <!-- START NAVBAR DESKTOP -->
      <nav id="navbar">
        <div class="img-container">
          <img src="../assets/logo/dropbox-icon.svg" alt="db_icon" />
          <img src="../assets/logo/dropbox-logo.svg" alt="Dropbox" />
        </div>

        <ul class="nav-list">
          <li class="nav-item dropdown-why dropdown">
            <a href="">Why Dropbox?</a>
            <ul id="why-features-menu" class="feature-menu">
              <ul class="why-feature-list feature-list">
                <li class="top-list-item"><a href="">Overview</a></li>
                <li><a href="">Costumer stories</a></li>
                <li><a href="">How we integrate</a></li>
                <li><a href="">Smart Workspace</a></li>
                <li><a href="">Do more than store</a></li>
              </ul>
              <ul class="why-feature-list feature-list">
                <li class="top-list-item"><a href="">By industry</a></li>
                <li><a href="">Education</a></li>
                <li><a href="">Media</a></li>
                <li><a href="">Construction</a></li>
                <li><a href="">Retail</a></li>
                <li><a href="">Technology</a></li>
              </ul>
              <ul class="why-feature-list feature-list">
                <li class="top-list-item"><a href="">By user type</a></li>
                <li><a href="">Personal</a></li>
                <li><a href="">Family</a></li>
                <li><a href="">Freelancers</a></li>
                <li><a href="">Teams</a></li>
                <li><a href="">Enterprice</a></li>
              </ul>
            </ul>
          </li>

          <li class="nav-item dropdown-feature dropdown">
            <a href="">Features</a>
            <ul id="feature-features-menu" class="feature-menu">
              <ul class="feature-feature-list feature-list">
                <li><a href="">Share files</a></li>
                <li><a href="">Store and back up</a></li>
                <li><a href="">Sync devices</a></li>
                <li><a href="">Simplify eSignatures</a></li>
                <li><a href="">Protect and secure</a></li>
                <li><a href="">Be productive</a></li>
              </ul>
              <ul class="feature-feature-list feature-list">
                <li><a href="">Get desktop app</a></li>
                <li><a href="">Get mobile app</a></li>
                <li><a href="">Work remotely</a></li>
                <li><a href="">Collaborate</a></li>
                <li><a href="">Organize a team</a></li>
              </ul>
            </ul>
          </li>

          <li class="nav-item"><a href="">Plans & pricing</a></li>

          <li class="nav-item divider dropdown-support dropdown">
            <a href="">Support</a>
            <ul id="support-features-menu" class="feature-menu">
              <ul class="support-feature-list feature-list">
                <li><a href="">Help center</a></li>
                <li><a href="">Community forums</a></li>
              </ul>
            </ul>
          </li>
          <li class="nav-item dropdown-vertrieb dropdown">
            <a href="">Contact sales</a>
            <ul id="vertrieb-features-menu" class="feature-menu">
              <ul class="vertrieb-feature-list feature-list">
                <li><a href="">Email</a></li>
                <li><a href="">Chat</a></li>
                <li><a href="">1 (855) 237-6726</a></li>
              </ul>
            </ul>
          </li>

          <li class="nav-item"><a href="">Sign in</a></li>
        </ul>

        <div class="start-button">
          <button>Get started</button>
        </div>
      </nav>
      <!-- END NAVBAR DESKTOP -->
      <!-- START NAVBAR MOBILE -->
      <nav id="navbar-mobile">
        <div class="img-container">
          <img src="../assets/logo/dropbox-icon.svg" alt="db_icon" />
          <img src="../assets/logo/dropbox-logo.svg" alt="Dropbox" />
        </div>
        <!-- <div class="nav-button-mobile"> -->
        <button id="nav-button" title="Menu toggle"></button>
        <!-- </div> -->
      </nav>
      <!-- END NAVBAR MOBILE -->
    </header>
    <!-- END HEADER -->
    <!-- START MAIN -->
    <main>
      <!-- START HERO -->
      <section class="hero">
        <h1>Everything you need for work, all in one place</h1>
        <div class="hero-cta">
          <button class="primary with-icon">
            Start your free trial
            <img src="../assets/icons/arrow.svg" alt="arrow icon" />
          </button>
          <span class="faint-text">Cancel any time</span>
        </div>
        <div class="action-text">
          <p>
            Finally now all your tools, content, and collaborators are
            accessible from the same place. Dropbox Business is more than secure
            storage—it's a smart, seamless way to optimize your existing
            workflow.
          </p>
        </div>
        <div class="hero-image">
          <img src="../assets/img/hero-image.png" alt="" />
        </div>
      </section>
      <!-- HANNES STARTS PRICING-->
      <section class="pricing">
        <div class="wrapper-header">
          <h2>Finde the Dropbox Business plan for you</h2>
        </div>
        <div class="wrapper-pricing">
          <div class="radios-billing">
            <label for="monthly-billing">
              <input
                checked
                type="radio"
                name="billing"
                id="monthly-billing"
                value="monthly"
              />
              Billed monthly</label
            >
            <label for="yearly-billing">
              <input
                type="radio"
                name="billing"
                id="yearly-billing"
                value="yearly"
              />
              Billed yearly</label
            >
          </div>
          <div class="pricing-options">
            <div id="pricing-professional">
              <div class="top-row-pricing">
                <div class="group-of-interest">
                  <img
                    class="icon-placing"
                    src="../assets/icons/individual.svg"
                    alt=""
                  />
                  <span>Individual</span>
                </div>
                <div>
                  <span class="pricing-option-name">Professional</span>
                </div>
                <div id="price-professional" class="price">$19.99</div>
                <div class="billing-option">/ month</div>
                <div class="free-trial-link">
                  <a href="https://www.dropbox.com/pro/try?hs=1"
                    >Try free for 30 days</a
                  >
                  <img src="../assets/icons/arrow.svg" alt="arrow icon" />
                </div>
                <div class="purchase-link">
                  <a href="https://www.dropbox.com/buy/professional?hs=1"
                    >Or purchase now</a
                  >
                </div>
              </div>
              <div class="contract-information">
                <div class="user-info">
                  <img
                    class="icon-placing"
                    src="../assets/icons/individual.svg"
                  /><span>1 user</span>
                </div>
                <div class="storage">
                  <img
                    class="icon-placing"
                    src="../assets/icons/folder.svg"
                  /><span>3 TB of secure storage</span>
                </div>
                <div class="collaboration-features">
                  <img
                    class="icon-placing"
                    src="../assets/icons/features.svg"
                  /><span
                    >Premium productivity features and simple, secure file
                    sharing</span
                  >
                </div>
              </div>
              <div class="plan-highlights">
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Send files up to 100 GB with Dropbox Transfer</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Mobile offline folder</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Remote account wipe</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Document watermarking</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Priority email and live chat support</div>
                </div>
              </div>
            </div>
            <div id="pricing-standard">
              <div class="top-row-pricing">
                <div class="group-of-interest">
                  <img src="../assets/icons/team.svg" alt="" />
                  <span>Team</span>
                </div>
                <div>
                  <span class="pricing-option-name">Standard</span>
                </div>
                <div id="price-standard" class="price">$15</div>
                <div class="billing-option">
                  / user / month, starting at 3 users
                </div>
                <div class="free-trial-link">
                  <a href="https://www.dropbox.com/pro/try?hs=1"
                    >Try free for 30 days</a
                  >
                  <img src="../assets/icons/arrow.svg" alt="arrow icon" />
                </div>
                <div class="purchase-link">
                  <a href="https://www.dropbox.com/buy/professional?hs=1"
                    >Or purchase now</a
                  >
                </div>
              </div>
              <div class="contract-information">
                <div class="user-info">
                  <img
                    class="icon-placing"
                    src="../assets/icons/individual.svg"
                  /><span>3+ users</span>
                </div>
                <div class="storage">
                  <img
                    class="icon-placing"
                    src="../assets/icons/folder.svg"
                  /><span>5 TB of secure storage</span>
                </div>
                <div class="collaboration-features">
                  <img
                    class="icon-placing"
                    src="../assets/icons/features.svg"
                  /><span
                    >Easy-to-use team management and colaboration tools</span
                  >
                </div>
              </div>
              <div class="plan-highlights">
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Single admin login to manage multiple teams</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Admin console and audit log</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>256-bit AES and SSL/TLS encryption</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Granular sharing permissions</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Priority email, live chat, and phone support</div>
                </div>
              </div>
            </div>
            <div id="pricing-advanced">
              <div class="top-row-pricing">
                <div class="group-of-interest">
                  <img src="../assets/icons/team.svg" alt="" />
                  <span>Team</span>
                </div>
                <div>
                  <span class="pricing-option-name">Advanced</span>
                </div>
                <div id="price-advanced" class="price">$25</div>
                <div class="billing-option">
                  / user / month, starting at 3 users
                </div>
                <div class="free-trial-link">
                  <a href="https://www.dropbox.com/pro/try?hs=1"
                    >Try free for 30 days</a
                  >
                  <img src="../assets/icons/arrow.svg" alt="arrow icon" />
                </div>
                <div class="purchase-link">
                  <a href="https://www.dropbox.com/buy/professional?hs=1"
                    >Or purchase now</a
                  >
                </div>
              </div>
              <div class="contract-information">
                <div class="user-info">
                  <img
                    class="icon-placing"
                    src="../assets/icons/individual.svg"
                  /><span>3+ users</span>
                </div>
                <div class="storage">
                  <img
                    class="icon-placing"
                    src="../assets/icons/folder.svg"
                  /><span>As much space as your team needs</span>
                </div>
                <div class="collaboration-features">
                  <img
                    class="icon-placing"
                    src="../assets/icons/features.svg"
                  /><span>
                    Sophisticated admin, audit, security, and integration
                    capabilities</span
                  >
                </div>
              </div>
              <div class="plan-highlights">
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Everything in Standard</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Advanced admin controls</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Tiered admin roles</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Single sign on (SSO) integration</div>
                </div>
                <div class="highlights-single-item">
                  <img src="../assets/icons/swoosh.svg" alt="" />
                  <div>Invite enforcement</div>
                </div>
              </div>
            </div>
            <div id="pricing-enterprise">
              <div class="top-row-pricing">
                <div class="group-of-interest">
                  <img src="../assets/icons/team.svg" alt="" />
                  <span>Team</span>
                </div>
                <div>
                  <span class="pricing-option-name">Enterprise</span>
                </div>
                <div class="price">Contact Sales for pricing</div>
                <div class="enterprise-info">
                  <span
                    >Custom solutions and individualized support to help IT
                    professionals manage at scale.
                  </span>
                </div>
              </div>
              <div class="enterprise-contact">
                <div class="free-trial-link">
                  <a href="https://www.dropbox.com/pro/try?hs=1">Contact us</a>
                  <img src="../assets/icons/arrow.svg" alt="arrow icon" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- HANNES ENDS PRICING-->
      <section class="connect">
        <div class="connect-container">
          <div class="left-box">
            <div class="connect-header">
              <h2>Connect with a Dropbox partner</h2>
            </div>
            <div class="connect-info">
              <p>
                Find a trusted Dropbox and HelloSign partner. Get the solutions
                and services you need to achieve your business goals, including
                implementation, integration, and ongoing management and support.
              </p>
            </div>
            <div class="button">
              <button type="button">
                <a href="https://experience.dropbox.com/partner-locator"
                  >Find a partner</a
                >
                <i class="fas fa-arrow-right"></i>
              </button>
            </div>
          </div>
          <div class="right-box">
            <img src="../assets/img/partners.jpeg" />
          </div>
        </div>
      </section>

      <!-- START FEATURE-GRID -->
      <section class="feature-grid">
        <h2>Do more with Dropbox Business</h2>
        <div class="feature-box">
          <div class="feature">
            <img src="../assets/img/features_1.png" alt="" />
            <h4>Do less switching between tools</h4>
            <p>
              Tackle your everyday tasks with one tool. Create, edit, and share
              cloud content from Google Docs, Sheets, and Slides, Microsoft
              Office files, and Dropbox Paper right from Dropbox.
            </p>
          </div>
          <div class="feature">
            <img src="../assets/img/features_2.png" alt="" />
            <h4>Transform your folders</h4>
            <p>
              Dropbox brings your files and cloud content together, so that your
              PowerPoints can live next to your Google Docs, Trello boards, and
              any other files you may need.
            </p>
          </div>
          <div class="feature">
            <img src="../assets/img/features_3.png" alt="" />
            <h4>Collaboration, any time, anywhere</h4>
            <p>
              Easily access your team’s work from your computer, mobile device,
              or any web browser.
            </p>
          </div>
          <div class="feature">
            <img src="../assets/img/features_4.png" alt="" />
            <h4>Strike up a conversation</h4>
            <p>
              Leading communications tools, like Slack and Zoom, work right from
              Dropbox. Set up a quick touch-base—or even a virtual conference
              room—with just a few clicks.
            </p>
          </div>
          <div class="feature">
            <img src="../assets/img/features_5.png" alt="" />
            <h4>Securely send large files</h4>
            <p>
              Dropbox Transfer is the safe, easy way to deliver final files of
              any size to colleagues and clients. Set custom passwords and
              expiration dates to protect your work, and confirm delivery with
              download notifications.
            </p>
          </div>
          <div class="feature">
            <img src="../assets/img/features_6.png" alt="" />
            <h4>Get peace of mind</h4>
            <p>
              A
              <a
                href="https://www.dropbox.com/business/trust/security"
                target="_blank"
                >secure, distributed infrastructure</a
              >—plus
              <a
                href="https://www.dropbox.com/business/tour/administrative-tools"
                target="_blank"
                >admin tools</a
              >
              for control and visibility—keep your company’s data safe on
              Dropbox.
            </p>
          </div>
        </div>
      </section>
      <!-- END FEATURE-GRID -->

      <section class="testimonials">
        <div class="first-container">
          <h2 class="testimonials-title">
            More than 500,000 teams use Dropbox Business
          </h2>
          <a href="">Learn more about our customers</a>
        </div>
        <div class="second-container">
          <div class="logos">
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
            <img src="../assets/icons/designit-logo.svg" alt="" />
          </div>
          <div class="testimonial-container">
            <!-- <div class="right-arrow"><img src="../assets/icons/right-arrow.svg" alt=""></div>
          <div class="left-arrow"><img src="../assets/icons/left-arrow.svg" alt=""></div> -->
            <div class="testimonial-grid">
              <div class="grid-image">
                <img src="" alt="no image" id="testimonial-image" />
              </div>
              <div class="grid-text">
                <p id="testimonial-text"></p>
                <a href="" id="testimonial-link"></a>
                <p id="testimonial-person"></p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!--BELEN-->
      <section class="faq">
        <div class="faq-heading">
          <h2>Frequently asked questions</h2>
        </div>
        <ul>
          <li id="first-item">
            <button id="first-btn">
              <h4>
                What's the difference between Dropbox Business Standard and
                Dropbox Business Advanced?
              </h4>
              <img
                class="angle"
                id="angle-down"
                src="../assets/icons/angle-down-solid.svg"
                alt="angle-down"
              />
            </button>
            <p id="first-answer">
              Standard provides teams with 5 TB (5,000 GB) of storage, and
              simple sharing and collaboration tools. For teams needing more
              storage and security, Advanced provides as much space as your team
              needs in addition to sophisticated admin, audit, integration and
              security features. Learn more about our plans here.
            </p>
          </li>
          <li>
            <button>
              <h4>How much space does my team get?</h4>
              <img
                class="angle"
                id="angle-down"
                src="../assets/icons/angle-down-solid.svg"
                alt="angle-down"
              />
            </button>
            <p>
              Dropbox Business provides three plans to fit your team’s needs.
              The Standard plan gives your team 5 TB (5,000 GB) of shared
              storage. For teams needing more space, the Advanced and Enterprise
              plans provide as much space as you need.
            </p>
          </li>
          <li>
            <button>
              <h4>
                Can I upgrade my existing Basic or Plus account? How does
                migration work?
              </h4>
              <img
                class="angle"
                id="angle-down"
                src="../assets/icons/angle-down-solid.svg"
                alt="angle-down"
              />
            </button>
            <p>
              If you already use Dropbox, moving to a Dropbox Business account
              is easy! All of your content will stay the same – your files will
              stay where they are and all of your settings (such as shared
              folder relationships and linked devices) will remain the same. For
              admins, all of your team members who already use Dropbox will have
              the same experience, and anyone without an existing Dropbox
              account will be prompted to sign up when you send them an
              invitation. For Plus users who switch to Dropbox Business, any
              remaining credits will be returned as a pro rata refund to the
              original payment method.
            </p>
          </li>
          <li>
            <button>
              <h4>
                Do you have any discounts for Dropbox Business and Dropbox
                Enterprise?
              </h4>
              <img
                class="angle"
                id="angle-down"
                src="../assets/icons/angle-down-solid.svg"
                alt="angle-down"
              />
            </button>
            <p>
              Yes. We have volume discounts as well as discounts for non-profits
              and educational institutions. Please contact our sales team for
              more information.
            </p>
          </li>
        </ul>
      </section>
      <section class="trial">
        <div class="trial-container">
          <div class="trial-header">
            <h2>Bring Dropbox Business to your business</h2>
          </div>
          <div class="trial-button">
            <button type="button" id="trial-button">
              <a href="https://www.dropbox.com/business/plans-comparison"
                >Start your free trial</a
              >
              <i class="fas fa-arrow-right"></i>
            </button>
          </div>
        </div>
      </section>
    </main>
    <!-- END MAIN -->
    <footer></footer>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
// import Header from "@/components/Header.vue";

export default Vue.extend({
  components: {
    // Header
  }
});
</script>

<style scoped lang="scss"></style>
