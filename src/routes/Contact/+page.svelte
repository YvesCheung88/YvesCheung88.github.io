<form method="POST" class="contact-form">
	<h1>Formulaire de contact</h1>
	<div class="form-group">
		<label for="name" class="label-text">Name</label>
		<input type="text" id="name" aria-label="name" placeholder="Votre nom" class="input" required />
	</div>
	<div class="form-group">
		<label for="email" class="label-text">Email</label>
		<input
			type="email"
			id="email"
			aria-label="email"
			placeholder="Votre email"
			class="input"
			required
		/>
	</div>
	<div class="form-group">
		<label for="message" class="label-text">Message</label>
		<textarea name="message" id="message" aria-label="message" placeholder="Votre message"
		></textarea>
	</div>
	<button type="submit">Submit</button>
</form>

<style>
	.contact-form {
		display: flex;
		flex-direction: column;
		gap: 15px;
		border: 1px solid #ddd;
		border-radius: 8px;
	}
	.form-group {
		display: flex;
		flex-direction: column;
		gap: 10px;
	}
	.label-text {
		font-weight: bold;
		margin-bottom: 5px;
	}
</style>
