<template>
  <form
    name="Contact"
    method="post"
	netlify-honeypot="bot-field"
    data-netlify="true"
    >
    <!-- Name -->
    <div class="field">
      <label class="label is-medium">Name</label>
      <div class="control has-icons-left">
        <input class="input is-medium" type="text" placeholder="John Smith" name="name" />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="user" />
        </span>
      </div>
    </div>
    <!-- Email -->
    <div class="field">
      <label class="label is-medium">Email</label>
      <div class="control has-icons-left">
        <input
          class="input is-medium"
          type="email"
          placeholder="you@email.com"
          name="email"
        />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="envelope" />
        </span>
      </div>
    </div>
    <!-- Subject -->
    <div class="field">
      <label class="label is-medium">Subject</label>
      <div class="control has-icons-left">
        <input
          class="input is-medium"
          type="text"
          placeholder="Brief Summary"
          name="subject"
        />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="briefcase" />
        </span>
      </div>
    </div>
    <!-- Message -->
    <div class="field">
      <label class="label is-medium">Message</label>
      <div class="control">
        <textarea
          class="textarea"
          placeholder="Detailed description of your comment, request, etc"
          name="message"
          rows="8"
        ></textarea>
      </div>
    </div>
	<p hidden>
      <label>Don’t fill this out if you're human: <input name="bot-field" /></label>
    </p>
    <div class="control">
      <button class="button is-primary">
        Contact Us
      </button>
    </div>
  </form>
</template>
