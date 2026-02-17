<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Live Premium</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .neon-text {
      text-shadow: 0 0 5px #ff00cc, 0 0 10px #ff00cc, 0 0 20px #ff00cc;
    }
    .neon-box {
      box-shadow: 0 0 15px #ff00cc;
    }
  </style>
</head>
<body class="bg-black text-white font-sans overflow-x-hidden">

  <div class="fixed w-full h-full -z-10 opacity-40 animate-pulse"
style="
background: linear-gradient(45deg, #ff00cc, #333399, #ff00cc);
background-size: 400% 400%;
animation: gradientMove 6s ease infinite;
">
</div>

<style>
@keyframes gradientMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
</style>


  <section class="min-h-screen flex items-center justify-center px-6">
    <div class="max-w-4xl text-center">

      <div class="inline-block px-6 py-2 mb-6 rounded-full bg-red-600 animate-pulse text-sm tracking-widest">
        🔴 LIVE NOW
      </div>

      <div class="mb-8 flex justify-center">
        <img src="profile.gif" alt="Live Preview"
        class="rounded-2xl neon-box w-72 md:w-96 border-4 border-pink-600 object-cover">
      </div>

      <h1 class="text-4xl md:text-6xl font-bold mb-6 neon-text">
        PREMIUM LIVE ACCESS
      </h1>

      <p class="text-lg md:text-xl text-gray-300 mb-6">
        Private streaming • Exclusive content • VIP members only
      </p>

      <div class="mb-10 text-2xl font-semibold" id="countdown"></div>

      <div class="flex flex-col sm:flex-row gap-6 justify-center">
        <a href="https://www.liveroomcam.com/?utm_source=da57dc555e50572d&&ban=fb&s1=232783&s2=2110278&click_id=REWOSH-EDISI-RAMADHAN&ban" target="_blank"
          class="px-10 py-4 bg-green-500 text-black font-semibold rounded-2xl hover:scale-110 transition-transform duration-300">
          Join WhatsApp
        </a>

        <a href="https://www.liveroomcam.com/?utm_source=da57dc555e50572d&&ban=fb&s1=232783&s2=2110278&click_id=REWOSH-EDISI-RAMADHAN&ban"
          class="px-10 py-4 bg-pink-600 font-semibold rounded-2xl hover:scale-110 transition-transform duration-300">
          Order VIP
        </a>
      </div>
    </div>
  </section>

  <div id="chatPopup" class="fixed bottom-6 right-6 bg-gray-900 border border-pink-600 rounded-2xl p-4 w-64 shadow-2xl hidden">
    <p class="text-sm mb-2">💬 Admin sedang online</p>
    <a href="https://www.liveroomcam.com/?utm_source=da57dc555e50572d&&ban=fb&s1=232783&s2=2110278&click_id=REWOSH-EDISI-RAMADHAN&ban" target="_blank" class="text-green-400 underline">CONTINUE</a>
  </div>

  <footer class="py-6 text-center text-gray-500 text-sm border-t border-gray-800">
    © 2026 Premium Live. All Rights Reserved.
  </footer>

  <script>
    let time = 600;
    const countdownEl = document.getElementById('countdown');

    setInterval(() => {
      let minutes = Math.floor(time / 60);
      let seconds = time % 60;
      countdownEl.innerHTML = "⏳ Promo berakhir dalam: " + minutes + "m " + seconds + "s";
      if (time > 0) time--;
    }, 1000);

    setTimeout(() => {
      document.getElementById('chatPopup').classList.remove('hidden');
    }, 5000);
  </script>

</body>
</html>
