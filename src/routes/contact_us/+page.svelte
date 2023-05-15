
<main>
    <div class="flex justify-between mx-4 my-8">
    
      <div class="flex-1">
        <h2 class="text-4xl font-bold mb-10">Contact Us</h2>
        <p class="text-gray-600 mb-5">Have questions or feedback?</p>
        <p class="text-gray-600 mb-5">We would love to hear from you!</p>
        <p class="text-gray-600">Please contact us through our form, email, phone or visit us directly.</p>
      </div>
  
      <div class="flex-1">
        <h2 class="text-4xl font-bold mb-10">Send us a Message</h2>
        <form on:submit|preventDefault={handleSubmit}>
          <div class="mb-4">
            
            <input class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="name" type="text" placeholder="Name" bind:value={formData.name}>
          </div>
          <div class="mb-4">
            
            <input class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="email" type="email" placeholder="E-mail" bind:value={formData.email}>
          </div>
          <div class="mb-4">
            
            <input class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="website" type="text" placeholder="Website" bind:value={formData.website}>
          </div>
          <div class="mb-4">
            
            <textarea class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="message" rows="8" placeholder="Message" bind:value={formData.message}></textarea>
          </div>
          <div class="flex justify-end">
            <button class="bg-gray-700 text-white font-semibold py-2 px-5 rounded focus:outline-none focus:shadow-outline" type="submit">SUBMIT</button>
          </div>
        </form>
      </div>
    </div>
  </main>
  
  <script>
    let formData = {
      name: '',
      email: '',
      website: '',
      message: ''
    };
  
    function handleSubmit() {
      // Handle form submission here
      console.log(formData);
    }
  </script>
  