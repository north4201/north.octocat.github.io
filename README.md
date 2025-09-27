<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>You've Been Invited to SEELE AI</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Inter:wght@400;700&family=Source+Serif+4:opsz,wght@8..60,600&display=swap"
      rel="stylesheet"
    />
    <style>
      body { font-family: 'Inter', sans-serif; }
      .font-serif-display { font-family: 'Source Serif 4', serif; }
      .font-cursive { font-family: 'Great Vibes', cursive; }
      .bg-curves { position: fixed; top:0; left:0; width:100%; height:100%; z-index:-1; overflow:hidden; }
      .curve { position:absolute; border-radius:50%; border:1px solid rgba(255,255,255,0.05); animation:rotate 40s linear infinite; }
      .curve-1 { width:150vmax; height:150vmax; top:-50vmax; right:-50vmax; }
      .curve-2 { width:120vmax; height:120vmax; bottom:-60vmax; left:-20vmax; animation-direction:reverse; animation-duration:50s; }
      @keyframes rotate { from { transform:rotate(0deg); } to { transform:rotate(360deg); } }
      .copied-feedback { position:absolute; top:-35px; left:50%; transform:translateX(-50%); background-color:#059669; color:white; padding:4px 10px; border-radius:7px; font-size:0.875rem; font-weight:600; opacity:0; transition:opacity 0.3s ease, top 0.3s ease; white-space:nowrap; pointer-events:none; }
      .copied-feedback.show { opacity:1; top:-45px; }
    </style>
  </head>
  <body class="bg-black text-gray-200 flex items-center justify-center min-h-screen p-4 overflow-hidden">
    <div class="bg-curves">
      <div class="curve curve-1"></div>
      <div class="curve curve-2"></div>
    </div>

    <main class="w-full">
      <div id="loading-state" class="text-center">
        <div class="flex justify-center items-center">
          <div class="animate-spin rounded-full h-12 w-12 border-b-2 border-gray-400"></div>
        </div>
        <p class="mt-4 text-gray-400">Claiming your invitation...</p>
      </div>

      <div id="content-state" class="hidden">
        <div class="w-full max-w-5xl mx-auto flex flex-col lg:flex-row items-center justify-center gap-8 lg:gap-16 px-4">
          <div class="w-full max-w-xs sm:max-w-sm shrink-0 flex flex-col gap-4 order-2 lg:order-1">
            <di
