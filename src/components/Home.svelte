<main class="home">
	<div class="top"></div>
	<div class="container">
		<div class="bg_wrap">
			<img class="cool_bg" src="/images/bg-pattern-card.svg" alt="">
		</div>
		<div class="profile">
			<div class="circle">
				<img class="profile_img" src="/images/image-victor.jpg" alt="">
			</div>
			<div class="wrap">
				<h1 class="name">Victor Crest <span class="highlight">26</span></h1>
				<div class="location">London</div>
				<div class="line"></div>
				<div class="stat">
					<div class="col">
						<div class="value">80K</div>
						<div class="text">Followers</div>
					</div>
					<div class="col">
						<div class="value">803K</div>
						<div class="text">Likes</div>
					</div>
					<div class="col">
						<div class="value">1.4K</div>
						<div class="text">Photos</div>
					</div>
				</div>
			</div>		
		</div>
	</div>
	<div class="bottom"></div>
</main>

<style>
	.home {
		@apply w-screen h-screen bg-[#19a2ae] flex justify-center items-center bg-no-repeat;
		background-image: url('/images/bg-pattern-top.svg'), url("/images/bg-pattern-bottom.svg");
   		background-position: right 45vw bottom 45vh, 45vw 45vh;
	}
	.container {
		@apply w-[400px] h-[400px] rounded-[10px] bg-[#ffffff] flex flex-col items-center z-[10];
	}
	.bg_wrap {
		@apply w-[400px] h-[200px] rounded-tl-[10px] rounded-tr-[10px];
	}
	.cool_bg {
		@apply w-[100%] h-[175px] object-cover rounded-tl-[10px] rounded-tr-[10px];
	}
	.circle{
		@apply relative top-[-75px] w-[118px] h-[118px] bg-[#ffffff] rounded-[50%] flex justify-center items-center;
	}
	.profile_img {
		@apply w-[108px] h-[108px] rounded-[50%];
	}
	.profile {
		@apply w-[100%] flex flex-col items-center;
	}
	.wrap {
		@apply w-[100%] flex flex-col items-center relative top-[-60px];
	}
	.name, .value {
		@apply text-[18px] font-bold text-[#2d3248];
	}
	.stat {
		@apply flex flex-row gap-[45px];
	}
	.col {
		@apply flex flex-col items-center;
	}
	.location, .text, .highlight {
		@apply text-[16px] text-[#6a6f81];
	}
	.highlight {
		@apply inline-block;
	}
	.line {
		@apply w-[100%] h-[1px] mt-[24px] mb-[24px] bg-[#969696];
	}
	@media only screen and (max-width: 425px) {
		.container, .bg_wrap {
			width: 350px;
		}
	}
</style>