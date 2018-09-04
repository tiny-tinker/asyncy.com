<template>
  <div class="app-footer">
    <div class="container">
			<h1 class="display-1 text-center text-white mb-3">Time to write your story 🎉</h1>
			<h4 class="display-4 text-center text-white mb-5">Schedule a demo and build 3 applications in 15 minutes.</h4>
			<form class="d-flex mb-5">
				<div class="row w-100">
					<div class="col-8 col-md-9 col-lg-6 offset-lg-2">
						<a-input placeholder="Enter Email" inputClasses="bg-dark border-0" />
					</div>
					<div class="col-4 col-md-3 col-lg-2">
						<a-button type="neutral" class="w-100">Join Beta</a-button>
					</div>
				</div>
			</form>
			<div class="row">
				<div class="col-md-12 col-lg-3">
					<div class="menu-header">Product</div>
					<ul class="ul">
						<li class="li"><a href='https://asyncy.com/platform'>Platform</a></li>
						<li class="li"><a href='https://docs.asyncy.com'>Documentation</a></li>
						<li class="li"><a href='https://docs.asyncy.com/faq'>FAQ</a></li>
						<li class="li">
								<a href="https://asyncy.click/feedback" target="_blank" rel="noopener">Give Feedback</a>
						</li>
					</ul>
				</div>

				<div class="col-md-12 col-lg-3">
					<div class="menu-header">Resources</div>
					<ul class="ul">
						<li class="li"><a href='https://asyncy.com/events'>Events</a></li>
						<li class="li"><a href='https://medium.com/asyncy'>Blog</a></li>
					</ul>
				</div>

				<div class="col-md-12 col-lg-3">
					<div class="menu-header">Company</div>
					<ul class="ul">
						<li class="li"><a href='https://asyncy.com//about'>About</a></li>
						<li class="li"><a href='https://angel.co/asyncy/jobs'>Jobs</a></li>
						<li class="li"><a href='https://asyncy.com/contact'>Contact</a></li>
					</ul>
				</div>
				<div class="col-md-12 col-lg-3">
					<div class="socials">
						<a href='http://asyncy.click/slack' target="_blank" rel="noopener">
							<img :src="slackLogo" :style="{
								display: 'inline-block',
								width: '30px',
								opacity: 0.8,
							}" alt="Slack"/>
						</a>
						<a href='https://github.com/asyncy' target="_blank" rel="noopener">
							<img :src="githubLogo" :style="{
								display: 'inline-block',
								width: '30px',
								marginLeft: '25px',
								opacity: 0.8,
							}" alt="Github"/>
						</a>
						<a href='https://twitter.com/asyncy' target="_blank" rel="noopener">
							<img :src="twitterLogo" :style="{
								display: 'inline-block',
								width: '30px',
								marginLeft: '25px',
								opacity: 0.8,
							}" alt="Twitter"/>
						</a>
					</div>
					<div class="copyright">
						© 2018 Asyncy, Inc.
					</div>
				</div>
			</div>
    </div>
		<p class="h6 text-center color-white w-100 mt-5">Passionately built with <span class="color-red">❤</span> in Amsterdam</p>
  </div>
</template>

<script>
import slackLogo from '../../assets/img/slack_logo.svg';
import githubLogo from '../../assets/img/github_logo.svg';
import twitterLogo from '../../assets/img/twitter_logo.svg';

export default {
  data() {
    return {
      slackLogo,
      githubLogo,
      twitterLogo,
    };
  }
}
</script>

<style scoped lang="scss">
.app-footer {
  font-family: Graphik Web,-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif;
  background: url('../../assets/img/footer.jpg');
  font-size: 0.9em;
  padding-top: 75px;
  padding-bottom: 55px;
}

.app-footer .columns {
  max-width: 1000px;
  margin: 0 auto;
  padding: 0 25px;
}

.ul {
  list-style: none;
  padding-left: 0;
  text-align: left;
}

.li {
  font-size: 1.1em;
  margin-bottom: 0.5em;
}

.li a {
  color: #A3A3A3;
  font-size: 0.95em;
  font-weight: 400;
  line-height: 1.6em;
  text-decoration: none;
}

.li a:hover {
  color: white;
  transition: color 0.3s ease-out;
  -webkit-transition: color 0.3s ease-out;
  -moz-transition: color 0.3s ease-out;
  -o-transition: color 0.3s ease-out;
  transition: color 0.3s ease-out;
}

.menu-header {
  font-size: 1em;
  color: white;
  margin-bottom: 1em;
  text-align: left;
}

.copyright {
  color: #888;
  margin-top: 1em;
}

.socials {
	display: flex;
	align-items: center;
}
</style>
