<h1><slot /></h1>

<style>
	h1 {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		text-align: center;
		font-size: 3rem;
		text-decoration: underline;
		width: 100%;
		background-color: var(--color-surface);
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		padding: 1rem;
		margin-top: var(--margin-top, '');
		margin-bottom: var(--margin-bottom, '');
	}
</style>
