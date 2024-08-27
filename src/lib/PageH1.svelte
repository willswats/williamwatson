<h1><slot /></h1>

<style>
	h1 {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		text-align: center;
		font-size: 3rem;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 1rem 2rem;
		padding: 1rem;
	}

	@media screen and (max-width: 768px) {
		h1 {
			margin: 1rem;
		}
	}
</style>
