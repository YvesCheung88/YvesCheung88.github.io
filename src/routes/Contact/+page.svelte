<script>
	import { User, Mail } from 'lucide-svelte';
</script>

<form action="https://formsubmit.co/yves.cheung.88@gmail.com" method="POST">
	<h1>Formulaire de contact</h1>

	<div class="form-group">
		<label for="name" class="label-text">Name</label>
		<div class="input-icon">
			<span class="icon"><User /></span>
			<input
				type="text"
				id="name"
				aria-label="name"
				placeholder="Votre nom"
				class="input"
				required
			/>
		</div>
	</div>
	<div class="form-group">
		<label for="email" class="label-text">Email</label>
		<div class="input-icon">
			<span class="icon"> <Mail /> </span>

			<input
				type="email"
				id="email"
				aria-label="email"
				placeholder="Votre email"
				class="input"
				required
			/>
		</div>
	</div>

	<div class="form-group">
		<label for="message" class="label-text">Message</label>
		<textarea name="message" id="message" aria-label="message" placeholder="Votre message"
		></textarea>
	</div>
	<button type="submit">Submit</button>
</form>

<style>
	h1 {
		font-size: 2rem;
		margin-bottom: 1rem;
	}
	form {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		padding: 2rem;
		border-radius: 8px;
		max-width: 900px;
		margin: auto;
	}
	.form-group {
		display: flex;
		flex-direction: column;
	}
	.input-icon {
		position: relative;
		display: flex;
		align-items: center;
	}
	.icon {
		position: absolute;
		left: 10px;
	}
	.input {
		width: 100%;
		font-size: 1rem;
		border: 1px solid #9f1414;
		padding: 0.75rem 0.75rem 0.75rem 2.5rem;
	}
	textarea {
		padding: 0.75rem;
		font-size: 1rem;
		border: 1px solid #9f1414;
		border-radius: 8px;
	}

	.label-text {
		font-weight: bold;
		margin-bottom: 10px;
	}

	textarea {
		height: 15vh;
	}

	button {
		border: 1px solid #9f1414;
		border-radius: 8px;
		padding: 10px;
	}
</style>
