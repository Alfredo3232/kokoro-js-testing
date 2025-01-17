<template>
  <h1 style="color: whitesmoke">Kokoro JS</h1>

  <form>
    <div class="container">
      <div class="form-group">
        <label for="parser1">Insert Your Text Here</label>
        <input type="text" id="parser1" />
      </div>

      <div class="form-group">
        <label for="fileParser">Upload Your File Here</label>
        <input type="file" id="fileParser" />
      </div>
    </div>
  </form>
</template>

<script>
  import { KokoroTTS } from "kokoro-js";
  const model_id = "onnx-community/Kokoro-82M-ONNX";

  // const tts = await KokoroTTS.from_pretrained(model_id, {
  //   dtype: "q8", // Options: "fp32", "fp16", "q8", "q4", "q4f16"
  // });

  // const text = "Life is like a box of chocolates. You never know what you're gonna get.";
  // const audio = await tts.generate(text, {
  //   // Use `tts.list_voices()` to list all available voices
  //   voice: "af_bella",
  // });
  // audio.save("audio.wav");

  export default {};
</script>

<style>
  body {
    background-color: rgb(37, 37, 37);
  }

  .container {
    width: 40vw;
    height: 30vw;
    background-color: whitesmoke;
    border-radius: 10px;
    display: flex;
    flex-wrap: wrap;
    padding: 20px;
  }

  .form-group {
    flex: 1;
    margin-bottom: 10px;
  }
</style>
