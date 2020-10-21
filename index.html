<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Read 4 me</title>
    <link
      href="https://unpkg.com/tailwindcss/dist/tailwind.min.css"
      rel="stylesheet"
    />
    <script
      src="https://cdn.jsdelivr.net/gh/alpinejs/alpine@v2.x.x/dist/alpine.min.js"
      defer
    ></script>

    <style>
      @import url("https://fonts.googleapis.com/css?family=Montserrat");

      body,
      button,
      textarea {
        font-family: "Montserrat";
      }

      #container {
          width: min(90%, 400px);
          margin: auto;
      }

      textarea {
        width: 90%;
        height: calc(100vh - 212px);
      }
    </style>
  </head>

  <body
    class="m-auto text-center min-h-full bg-black text-white"
    x-data="speech()"
    @keydown.space="toggleSpeak"
    @keydown="speed"
  >
    <div id="container">
        <header class="border-b p-4">
            <h1 class="text-sm">LEIA PARA MIM</h1>
          </header>
      
          <main>
            <textarea
              class="border border-purple-500 m-4 text-black"
              @input="setText"
              placeholder="Coloque o texto aqui..."
            ></textarea>
          </main>
      
          <footer class="fixed inset-x-0 bottom-0 p-4">
            <button
              class="p-8 bg-yellow-400 text-black rounded-full shadow"
              @click="toggleSpeak"
            >
              <svg
                :hidden="isSpeaking"
                viewBox="0 0 24 24"
                width="24"
                height="24"
                stroke="currentColor"
                stroke-width="2"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="css-i6dzq1"
              >
                <polygon points="5 3 19 12 5 21 5 3"></polygon>
              </svg>
              <svg
                :hidden="!isSpeaking"
                viewBox="0 0 24 24"
                width="24"
                height="24"
                stroke="currentColor"
                stroke-width="2"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="css-i6dzq1"
              >
                <rect x="6" y="4" width="4" height="16"></rect>
                <rect x="14" y="4" width="4" height="16"></rect>
              </svg>
            </button>
            <!-- <button class="p-8 pt-2 pb-2 bg-red-600 rounded text-red-100" @click="stop">Parar</button> -->
            <div class="mt-4 text-sm" :disabled="isSpeaking">
              <button
                class="p-4 pt-2 pb-2 rounded bg-yellow-400 shadow text-black"
                @click="decreaseSpeed"
              >
                -
              </button>
              Speed <span x-text="currentSpeed"></span>
              <button
                class="p-4 pt-2 pb-2 rounded bg-yellow-400 shadow text-black"
                @click="increaseSpeed"
              >
                +
              </button>
            </div>
          </footer>
    </div>

    <script>
      function speech() {
        return {
          isSpeaking: false,
          currentSpeed: 3,
          synth: speechSynthesis,
          utterance: null,
          text: null,
          setText(event) {
            this.text = event.currentTarget.value;
          },
          init() {
            this.utterance = new SpeechSynthesisUtterance();
            this.utterance.lang = "pt-BR";
            this.utterance.rate = this.currentSpeed;
            this.utterance.text = this.text;
            this.utterance.onend = this.finishedSpeak.bind(this);
          },

          speak() {
            this.isSpeaking = true;

            this.init();
            this.synth.speak(this.utterance);
          },

          stop() {
            this.isSpeaking = false;

            this.synth.cancel();
          },

          toggleSpeak() {
            this.isSpeaking = !!this.isSpeaking;
            console.log("toggleSpeak", this.isSpeaking);
            //this.isSpeaking ? this.synth.pause() : this.synth.resume();
            this.isSpeaking ? this.stop() : this.speak();
          },

          speed(e) {
            if (e.key == "d") {
              this.increaseSpeed();
            }
            if (e.key == "s") {
              this.decreaseSpeed();
            }
          },

          increaseSpeed() {
            this.currentSpeed = +(this.currentSpeed + 0.1).toFixed(1);
          },

          decreaseSpeed() {
            this.currentSpeed = +(this.currentSpeed - 0.1).toFixed(1);
          },

          finishedSpeak() {
            this.isSpeaking = false;
          },
        };
      }
    </script>
  </body>
</html>
