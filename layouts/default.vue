<template>
	<div class="container">
		<header class="main-header">
			<nav class="navigation">
				<h3 class="logo">Logo</h3>
				<!-- <NuxtLink to="/" class="font-bold">Nuxt Dojo</NuxtLink> -->
				<ul class="navigation-list">
					<li>
						<NuxtLink to="/">Home</NuxtLink>
					</li>
					<li>
						<NuxtLink to="/about">About</NuxtLink>
					</li>
					<li>
						<NuxtLink to="/pricing">Pricing</NuxtLink>
					</li>
					<li>
						<NuxtLink to="/facts">Facts</NuxtLink>
					</li>
					<li>
						<NuxtLink to="/blog">Blog</NuxtLink>
					</li>
					<li>
						<NuxtLink to="/support">Support</NuxtLink>
					</li>
					<li class="download-app-button" @click="downloadApplication">
						Download
					</li>
					<li class="change-language-button" @click="changeLanguage">Eng</li>
				</ul>
			</nav>
		</header>
		<div class="content-wrapper">
			<slot/>
		</div>
	</div>
	<div class="footer-wrapper">
		<footer class="footer-main">
			<h3 class="logo">Logo</h3>
			<div class="links-first">
				<div>About Us</div>
				<div>Blog</div>
				<div>Support</div>
			</div>
			<div class="links-second">
				<div>Terms & Conditions</div>
				<div>Privacy Policy</div>
				<div>Cookies</div>
			</div>
			<div class="links-icons">
				<img src="~/assets/svg/facebook-icon.svg" alt="facebook-icon"/>
				<img src="~/assets/svg/instagram-icon.svg" alt="instagram-icon"/>
				<img src="~/assets/svg/youtube-icon.svg" alt="youtube-icon"/>
				<img src="~/assets/svg/pinterest-icon.svg" alt="pinterest-icon"/>
			</div>
		</footer>
	</div>
</template>

<script setup>
const downloadApplication = () => {
	console.log ('Download Application!');
};
const changeLanguage = () => {
	console.log ('Change language action!');
};
</script>

<style scoped>
.container {
	max-width: 1240px;
	margin: 0 auto;
}

.main-header {
	height: 100px;
	display: flex;
}

.navigation {
	width: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.logo {
	text-transform: uppercase;
	color: var(--color-accent);
	font-size: 40px;
	font-style: normal;
	font-weight: 700;
	line-height: normal;
}

.navigation-list {
	display: flex;
	align-items: center;
}

.navigation-list li {
	font-size: 18px;
	font-style: normal;
	font-weight: 400;
	line-height: 28px;
	margin-left: 24px;
}

.navigation-list li a:visited {
	color: var(--text-color-primary);
}

.navigation-list li a:active,
.navigation-list li a:hover {
	color: var(--color-accent);
}

.navigation-list li.download-app-button {
	display: flex;
	width: 174px;
	height: 44px;
	padding: 10px 24px;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	gap: 10px;
	flex-shrink: 0;
	border-radius: 100px;
	background-color: var(--color-accent);
	color: #fff;
	cursor: pointer;
}

.change-language-button {
	cursor: pointer;
}

.navigation-list li.download-app-action a:visited,
.navigation-list li.download-app-action a:hover,
.navigation-list li.download-app-action a:active {
	color: #fff;
}

.footer-wrapper {
	height: 302px;
	padding-top: 80px;
	background-color: #423c4e;
	margin-top: 160px;
}

.footer-main {
	max-width: 1240px;
	margin: 0 auto;
	display: flex;
	justify-content: space-between;
}

.footer-main > div {
	color: #fff;
	margin-right: 92px;
	font-size: 24px;
	font-style: normal;
	font-weight: 400;
	line-height: 50px;
}

.footer-main > div:last-child {
	margin-right: 194px;
	margin-top: 12px;
}

.footer-main .logo {
	color: #fff;
	margin-right: 92px;
}

.links-icons img {
	margin-right: 20px;
}

.links-icons img:last-child {
	margin-right: 0;
}
</style>
