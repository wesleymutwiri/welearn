<script>
	import { page } from '$app/stores';
</script>

<div class="sidebar">
	<div class="sidebar-top">
		<a class="sidebar-header" href="/">Welearn</a>
		<div class="sidebar-links">
			<a href="#" class="sidebar-link" class:active={$page.path === '/'}> Home </a>
			<a href="#" class="sidebar-link">
				<svg
					height="24"
					viewBox="0 0 74 74"
					width="24"
                    stroke="currentColor"
					stroke-width="2"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
					><path
						d="m11.23 64.92a1 1 0 0 1 -1-1v-53.92a8.009 8.009 0 0 1 8-8h2.77a1 1 0 0 1 0 2h-2.77a6.006 6.006 0 0 0 -6 6v53.92a1 1 0 0 1 -1 1z"
					/><path
						d="m62.77 57.84h-41.77a1 1 0 0 1 -1-1v-53.84a1 1 0 0 1 1-1h41.77a1 1 0 0 1 1 1v53.84a1 1 0 0 1 -1 1zm-40.77-2h39.77v-51.84h-39.77z"
					/><path
						d="m62.77 72h-44.46a8.08 8.08 0 0 1 0-16.16h44.46a1 1 0 0 1 1 1v14.16a1 1 0 0 1 -1 1zm-44.46-14.16a6.08 6.08 0 0 0 0 12.16h43.46v-12.16z"
					/><path
						d="m54 25h-24.23a1 1 0 0 1 -1-1v-10a1 1 0 0 1 1-1h24.23a1 1 0 0 1 1 1v10a1 1 0 0 1 -1 1zm-23.23-2h22.23v-8h-22.23z"
					/><path d="m53.458 64.92h-32.916a1 1 0 0 1 0-2h32.916a1 1 0 0 1 0 2z" /></svg
				>
				My Courses
			</a>
			<a href="#" class="sidebar-link">
				<svg
					viewBox="0 0 24 24"
					width="24"
					height="24"
					stroke="currentColor"
					stroke-width="2"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="css-i6dzq1"
					><path
						d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"
					/>
				</svg>
				Favourite
			</a>
			<a href="#" class="sidebar-link">Test</a>
			<a href="#" class="sidebar-link">Achievements</a>
			<a href="#" class="sidebar-link">Certificate</a>
			<a href="#" class="sidebar-link">Settings</a>
		</div>
	</div>
	<div class="sidebar-footer">
		<img src="https://source.unsplash.com/1600x900/?male" alt="" class="sidebar-footer-avatar" />
		<div class="sidebar-footer-details">
			<h4>Wesley M.</h4>
			<p class="text-light">Premium account</p>
		</div>
		<div class="sidebar-footer-controls">
			<svg
				viewBox="0 0 24 24"
				width="20"
				height="20"
				stroke="currentColor"
				stroke-width="4"
				fill="none"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="css-i6dzq1"
				><polyline points="18 15 12 9 6 15" />
			</svg>
			<svg
				viewBox="0 0 24 24"
				width="20"
				height="20"
				stroke="currentColor"
				stroke-width="4"
				fill="none"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="css-i6dzq1"
				><polyline points="6 9 12 15 18 9" />
			</svg>
		</div>
	</div>
</div>

<style>
	.sidebar {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		height: 100%;
		min-height: 100vh;
		padding: 0 2rem;
		font-family: 'Poppins', sans-serif;
		width: 300px;
		box-shadow: 0px 0px 2px #2d2d2f;
	}

	.sidebar-header {
		color: black;
		font-size: 2rem;
		position: relative;
		display: block;
		margin: 3rem 0;
		text-decoration: none;
	}
	.sidebar-header::after {
		position: absolute;
		height: 40px;
		width: 40px;
		border-radius: 50%;
		background: #ea6c00;
		bottom: 0;
		right: 0;
		display: block;
	}
	.sidebar-links {
		display: flex;
		flex-direction: column;
	}
	.sidebar-link {
		display: flex;
		align-items: center;
		text-decoration: none;
		padding: 1rem 0;
		color: #808191;
	}
	.sidebar-link.active {
		background: #2f3ced;
		color: #fdfdfd;
		padding: 1rem 2rem;
		width: 240px;
		border-radius: 0 1rem 1rem 0;
		margin-left: calc(-2rem);
	}

	.sidebar-footer {
		display: flex;
		/* justify-content: space-evenly; */
		align-items: center;
		padding: 1rem 0;
	}
	.sidebar-footer-avatar {
		height: 40px;
		width: 40px;
		border-radius: 50%;
		margin-right: 1rem;
	}
	.sidebar-footer-details {
		margin-right: 1rem;
	}

	.sidebar-footer-controls {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.sidebar-footer-controls svg {
		margin: -3px 0;
	}
	.text-light {
		color: #808191;
	}
</style>
