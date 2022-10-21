<template>
  <div class="app noselect">
    <TopHeader/>
    <TheContents/>
    <TheSkils/>
	<TheFooter/>
  </div>
</template>

<script>
import TopHeader from './components/TopHeader.vue';
import TheContents from './components/TheContents.vue';
import TheSkils from './components/TheSkils.vue';
import TheFooter from './components/TheFooter.vue';
export default {
    name: "App",
    components: { TopHeader, TheContents, TheSkils, TheFooter }
}
</script>

<style>
html {
  @import url("//cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.4/dist/web/static/pretendard.css");
  @import url("//cdn.jsdelivr.net/gh/toss/tossface/dist/tossface.css");
	font-family: Pretendard, Tossface, -apple-system, BlinkMacSystemFont, system-ui, Roboto, "Helvetica Neue", "Segoe UI", "Apple SD Gothic Neo", "Noto Sans KR", "Malgun Gothic",
		"Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", sans-serif;
  font-size: 10px;
  margin: 1.2rem;
	background-color: #101010;
	color: rgb(243, 239, 231);
  margin: 0;
	padding: 0;
}
::-webkit-scrollbar {
	width: 7px;
	height: 3.5px;
}

::-webkit-scrollbar-thumb {
	background: rgba(221, 221, 221, 0.5);
	border-radius: 20px;
}
.noselect {
	-webkit-touch-callout: none;
	-webkit-user-select: none;
	-khtml-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none;
}
.app {
	position: absolute;
	width: 45%;
	left: 50%;
	padding: 1rem 0 3rem 0;
	transform: translate(-50%, 0);
	word-break: keep-all;
}
.app h1 {
	font-size: 3.5rem;
}
.app h2 {
	font-size: 3.2rem;
}
.app p {
	font-size: 2.4rem;
}
.app hr {
	width: 100%;
	height: 1px;
	border: none;
	background-color: rgba(243, 239, 231, 0.5);
	margin: 0.5rem 0 1rem 0;
}
.app li {
	font-size: 1.7rem;
	list-style: circle;
}
.app footer {
	color: #33cc33ad;
	font-size: 1.3rem;
	font-weight: 400;
	text-align: center;
	margin-top: 3rem;
}
.app footer a {
	color: #33cc33ad;
	text-decoration: none;
}

.link {
	display: flex;
	margin-top: 2rem;
}
.link li {
	float: left;
	list-style: none;

	margin-right: 1.5rem;
	font-weight: 500;
}
.link a {
	color: #949acf;
	text-decoration: none;
}

.subtitle {
	margin-bottom: 1rem;
	font-weight: 200;
}
.views {
	margin-bottom: 1rem;
}
.subsubtitle {
	font-weight: 300;
	margin-top: 2.5rem;
}
.gray {
	color: rgb(202, 197, 207);
}
.detail {
	font-weight: 300;
}

@media (max-width: 1180px) {
	.app {
		width: 65%;
	}
}
@media (max-width: 600px) {
	.app {
		width: 85%;
	}
}

.links a {
	color: #949acf;
	text-decoration: none;
	margin-top: 2rem;
	font-size: 1.5rem;
}
</style>
