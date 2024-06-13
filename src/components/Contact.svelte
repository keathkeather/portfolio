<script>
	import SectionWrapper from "./SectionWrapper.svelte";


</script>


<SectionWrapper id="Contact">
    <div class="flex flex-col gap-5 sm:gap-5 md:gap-5 flex-1  justify-center pb-10 md:pb-14 items-end">
        <div class="form-container">
            <form class="form">
              <div class="form-group">
                <label for="email">Email</label>
                <input  name="email" id="email" type="text">
              </div>
              <div class="form-group">
                <label for="textarea">How Can I Help You?</label>
                <textarea  cols="50" rows="10" id="textarea" name="textarea">          </textarea>
              </div>
              <button type="submit" class="button">Submit</button>
            </form>
          </div>
    </div>
</SectionWrapper>