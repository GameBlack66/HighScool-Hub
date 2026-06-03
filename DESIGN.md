<!DOCTYPE html>

<html lang="fr"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;800&amp;family=Plus+Jakarta+Sans:wght@400;600&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
            display: inline-block;
            line-height: 1;
            text-transform: none;
            letter-spacing: normal;
            word-wrap: normal;
            white-space: nowrap;
            direction: ltr;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 4px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: transparent;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #c3c6d7;
            border-radius: 10px;
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "primary-fixed": "#dbe1ff",
                      "on-secondary": "#ffffff",
                      "surface-container": "#eaedff",
                      "on-background": "#131b2e",
                      "outline": "#737686",
                      "surface-variant": "#dae2fd",
                      "on-secondary-container": "#fffbff",
                      "on-tertiary-fixed": "#3d0026",
                      "tertiary-container": "#b74082",
                      "tertiary-fixed-dim": "#ffafd3",
                      "background": "#faf8ff",
                      "surface-container-lowest": "#ffffff",
                      "surface-dim": "#d2d9f4",
                      "on-tertiary-fixed-variant": "#85145a",
                      "surface-container-low": "#f2f3ff",
                      "on-tertiary-container": "#ffecf1",
                      "on-surface": "#131b2e",
                      "tertiary": "#982669",
                      "surface-container-high": "#e2e7ff",
                      "on-error-container": "#93000a",
                      "on-tertiary": "#ffffff",
                      "primary-fixed-dim": "#b4c5ff",
                      "inverse-surface": "#283044",
                      "primary": "#004ac6",
                      "surface": "#faf8ff",
                      "surface-container-highest": "#dae2fd",
                      "primary-container": "#2563eb",
                      "surface-tint": "#0053db",
                      "on-secondary-fixed": "#23005c",
                      "inverse-on-surface": "#eef0ff",
                      "on-secondary-fixed-variant": "#5516be",
                      "error-container": "#ffdad6",
                      "on-primary-fixed": "#00174b",
                      "secondary-fixed-dim": "#d0bcff",
                      "inverse-primary": "#b4c5ff",
                      "error": "#ba1a1a",
                      "secondary": "#6b38d4",
                      "on-surface-variant": "#434655",
                      "outline-variant": "#c3c6d7",
                      "tertiary-fixed": "#ffd8e7",
                      "on-primary": "#ffffff",
                      "secondary-fixed": "#e9ddff",
                      "on-error": "#ffffff",
                      "on-primary-fixed-variant": "#003ea8",
                      "secondary-container": "#8455ef",
                      "on-primary-container": "#eeefff",
                      "surface-bright": "#faf8ff"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px"
              },
              "spacing": {
                      "lg": "48px",
                      "gutter": "24px",
                      "base": "8px",
                      "sm": "12px",
                      "xl": "80px",
                      "margin": "24px",
                      "md": "24px",
                      "xs": "4px"
              },
              "fontFamily": {
                      "headline-lg": ["Montserrat"],
                      "headline-md": ["Montserrat"],
                      "headline-xl": ["Montserrat"],
                      "headline-xl-mobile": ["Montserrat"],
                      "label-md": ["Plus Jakarta Sans"],
                      "body-md": ["Plus Jakarta Sans"],
                      "headline-lg-mobile": ["Montserrat"],
                      "body-lg": ["Plus Jakarta Sans"]
              },
              "fontSize": {
                      "headline-lg": ["32px", {"lineHeight": "1.2", "fontWeight": "700"}],
                      "headline-md": ["24px", {"lineHeight": "1.3", "fontWeight": "700"}],
                      "headline-xl": ["48px", {"lineHeight": "1.1", "letterSpacing": "-0.02em", "fontWeight": "800"}],
                      "headline-xl-mobile": ["32px", {"lineHeight": "1.2", "letterSpacing": "-0.02em", "fontWeight": "800"}],
                      "label-md": ["14px", {"lineHeight": "1.4", "letterSpacing": "0.05em", "fontWeight": "600"}],
                      "body-md": ["16px", {"lineHeight": "1.6", "fontWeight": "400"}],
                      "headline-lg-mobile": ["24px", {"lineHeight": "1.2", "fontWeight": "700"}],
                      "body-lg": ["18px", {"lineHeight": "1.6", "fontWeight": "400"}]
              }
            },
          },
        }
    </script>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-background text-on-surface font-body-md custom-scrollbar overflow-x-hidden pb-24">
<!-- TopAppBar -->
<header class="bg-surface dark:bg-on-background w-full top-0 sticky shadow-sm dark:shadow-none z-50">
<div class="flex justify-between items-center px-margin h-16 w-full max-w-full">
<div class="flex items-center gap-3">
<div class="w-10 h-10 rounded-full bg-primary-container flex items-center justify-center overflow-hidden border-2 border-white shadow-sm">
<img alt="Student Profile Avatar" class="w-full h-full object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuB7IhfPfCoYwB4pVMiuMhMysaSoD9mXVF4ULQgHIPlNEIQCpeCIOxGDJi1Vt7FSf9RgCQQDOT2x8vuI84hBGIw_AGsPu8ygf4CENQoLnRzzwbrgfHmDLECWRebe_4GtLv0Jmw_HdkrkUgGwSsm6P6vB_s4A0hbVcfdKFqDLUY9R--l_-LVhEK6iWW469oodtNqFcZoUEJ3N_XOxQZIEHoqk2bxiTNzrsQmb8p9sl3JXC8OvcEQDT-l39-tJd5jZ2T_wIbiwgzayyJ7b"/>
</div>
<h1 class="font-headline-lg-mobile text-headline-lg-mobile text-primary dark:text-primary-fixed tracking-tight">HighSchool Hub</h1>
</div>
<div class="flex items-center gap-4">
<button class="text-primary dark:text-primary-fixed hover:opacity-80 transition-opacity active:scale-95 transition-transform duration-200">
<span class="material-symbols-outlined text-2xl">notifications</span>
</button>
</div>
</div>
</header>
<main class="max-w-[1280px] mx-auto px-margin pt-base">
<!-- Search & Filter Section -->
<section class="py-md flex flex-col gap-sm">
<div class="relative group">
<span class="material-symbols-outlined absolute left-4 top-1/2 -translate-y-1/2 text-outline group-focus-within:text-primary transition-colors">search</span>
<input class="w-full h-14 pl-12 pr-4 rounded-xl border border-outline-variant bg-surface-container-low focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent transition-all font-body-md shadow-sm" placeholder="Rechercher un jeu..." type="text"/>
</div>
<div class="flex gap-2 overflow-x-auto pb-2 no-scrollbar">
<button class="px-6 py-2 rounded-full bg-primary text-on-primary font-label-md transition-all active:scale-95 whitespace-nowrap">Tous</button>
<button class="px-6 py-2 rounded-full bg-surface-container-high text-on-surface-variant font-label-md hover:bg-surface-variant transition-all active:scale-95 whitespace-nowrap">Action</button>
<button class="px-6 py-2 rounded-full bg-surface-container-high text-on-surface-variant font-label-md hover:bg-surface-variant transition-all active:scale-95 whitespace-nowrap">Puzzle</button>
<button class="px-6 py-2 rounded-full bg-surface-container-high text-on-surface-variant font-label-md hover:bg-surface-variant transition-all active:scale-95 whitespace-nowrap">Rétro</button>
<button class="px-6 py-2 rounded-full bg-surface-container-high text-on-surface-variant font-label-md hover:bg-surface-variant transition-all active:scale-95 whitespace-nowrap">Sports</button>
</div>
</section>
<!-- Bento Grid Highlight Section -->
<section class="mb-lg">
<h2 class="font-headline-md text-headline-md mb-sm text-on-surface">À la une</h2>
<div class="grid grid-cols-1 md:grid-cols-3 gap-md">
<!-- Large Featured Card -->
<div class="md:col-span-2 relative h-[300px] md:h-[400px] rounded-2xl overflow-hidden group shadow-lg">
<img class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700" data-alt="A high-intensity gaming action shot with neon blue and purple lights illuminating a professional gaming setup. The mood is electric and competitive, set in a dark room with vibrant digital effects swirling around a sleek controller. A modern, energetic HighSchool Hub aesthetic with sharp focus and cinematic lighting." src="https://lh3.googleusercontent.com/aida-public/AB6AXuBgWIq6tiVggKde7g3r5z6I0JPLzTUBSaH2oCO9FnbiYEvK1JGsbjMQ96u7JIgXE-vQBi6OpH9DqFs1Z_FClRjxKZXmFE-bPkp0Ta2MSMIdEK6VSR6Pc5LQjWAjLm-zZCEauZumfyRR30KSSFF-LUIitVINY5MSF4nVY6x0CAeZwcSgsemqoB0B1oqtrEkWnC0og9PpLgcbiEoCSKEdfpER0PWzOA-v7CU8mmZxZs_ZLSyxErMTKbfh3nQyxeDMuK94YqRcLvnp0mFD"/>
<div class="absolute inset-0 bg-gradient-to-t from-on-background/90 via-transparent to-transparent flex flex-col justify-end p-md">
<div class="flex items-center gap-2 mb-2">
<span class="px-3 py-1 rounded-full bg-tertiary text-on-tertiary text-xs font-bold uppercase tracking-wider">Populaire</span>
</div>
<h3 class="font-headline-lg text-headline-lg-mobile md:text-headline-lg text-white mb-2">Cyber Pulse: High School Elite</h3>
<p class="text-surface-variant mb-6 max-w-md line-clamp-2">Affrontez vos camarades dans ce jeu de course futuriste ultra-rapide. Grimpez dans le classement du lycée !</p>
<button class="w-fit px-8 py-3 rounded-xl bg-primary text-on-primary font-headline-md flex items-center gap-2 hover:bg-primary-container active:scale-95 transition-all shadow-xl">
<span class="material-symbols-outlined">play_arrow</span>
                            Jouer maintenant
                        </button>
</div>
</div>
<!-- Secondary Featured -->
<div class="flex flex-col gap-md">
<div class="relative flex-1 rounded-2xl overflow-hidden group shadow-md border border-outline-variant/20">
<img class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700" data-alt="A collection of colorful geometric puzzle pieces in vibrant purple and bright blue, floating in a clean, minimalist 3D space. The lighting is soft and high-key, creating a professional and sophisticated educational game vibe. The atmosphere is calm and focused, with a sleek, modern app interface feel." src="https://lh3.googleusercontent.com/aida-public/AB6AXuCl0zwmYh52BLKIliGubgRsvNR9OhYU4xv7JKCnCZrjuEVwBoJVYBoynAI2jTf6s-E4JFSCRes3fNXGwjjb93Ur6__fgYeUfIOb-wX72yz6nw7LaSez0CJUOD2IxbUyRit1JxAxBdxY2EQ82a_aElV9cRWey1mJfdrtavHivyXRugBIf1SafW5LpB2khU8mN0NkOxh-NsmFaVohOXcErhHZX1bkSy6CLxOxLTxATmB3vB6GVtxVglK2dvq8oOR3Lv_oMn7JwUsy2Tq5"/>
<div class="absolute inset-0 bg-gradient-to-t from-on-surface/80 to-transparent flex flex-col justify-end p-sm">
<h4 class="font-headline-md text-white text-body-lg">Logique Master</h4>
<p class="text-white/80 text-sm mb-2">Puzzle • 150 Niveaux</p>
<button class="bg-white/20 backdrop-blur-md text-white px-4 py-2 rounded-lg text-sm font-bold hover:bg-white/30 transition-colors">Lancer</button>
</div>
</div>
<div class="relative flex-1 rounded-2xl overflow-hidden group shadow-md border border-outline-variant/20">
<img class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700" data-alt="A nostalgic 8-bit retro gaming aesthetic featuring a classic pixelated landscape with a vibrant sunset of pinks and oranges. The scene is framed like a vintage arcade screen with soft glowing scanlines. The mood is nostalgic yet energetic, perfectly fitting a modern high school arcade section." src="https://lh3.googleusercontent.com/aida-public/AB6AXuCDZD20ibpV57kLBanxFguNb-T-pBrPh7NljcyoVKivjyevo2EhsF-TvbEVj1G_AjMyqaPMIBFMPtt675sqfQu7S1sYvrk-fgFIQv1VZ3SIx-NhvNMxpSd4wB2KcHwnWzjdYNQPwfhp33XPuN0pnO69XPoyapl1-QdJgtzIWGJ6DpJUZZChsDZboO1CVzTGuV8nfilsaV3MCLN-Rpx-kJa4I99NrXZvI1rUEfTYChTrALm_OIkRyZrEDI7Q82DPZU2mweEPfGG9wvGt"/>
<div class="absolute inset-0 bg-gradient-to-t from-on-surface/80 to-transparent flex flex-col justify-end p-sm">
<h4 class="font-headline-md text-white text-body-lg">Pixel Quest</h4>
<p class="text-white/80 text-sm mb-2">Rétro • Aventure</p>
<button class="bg-white/20 backdrop-blur-md text-white px-4 py-2 rounded-lg text-sm font-bold hover:bg-white/30 transition-colors">Lancer</button>
</div>
</div>
</div>
</div>
</section>
<!-- Main Categories Grid -->
<section class="pb-xl">
<div class="flex justify-between items-center mb-sm">
<h2 class="font-headline-md text-headline-md text-on-surface">Bibliothèque Complète</h2>
<button class="text-primary font-label-md flex items-center gap-1 hover:underline">Voir tout <span class="material-symbols-outlined text-sm">arrow_forward</span></button>
</div>
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-gutter">
<!-- Game Card 1 -->
<div class="bg-surface-container-lowest rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all group flex flex-col border border-outline-variant/30">
<div class="h-48 overflow-hidden relative">
<img class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" data-alt="A stylized digital illustration of a soccer match in progress under bright stadium lights. The art style is clean and energetic with bold strokes and a vibrant palette of primary blue and electric green. The mood is high-tempo and exciting, capturing a professional sports game atmosphere for students." src="https://lh3.googleusercontent.com/aida-public/AB6AXuCGgUdmD_HzSsFmJ8platz9-tg0511yiCd2YMiuoH7SNPIFDqFress3Q76pwTyD8de06L1ZbdSkkRgh2sp4kYOgOnjXdzwQHzfDhLUdOfHDqacLydz-BZEiTzjcB5eomqM6CqwOPBjCTQ1i5TJvtRZTBIelzqIRzYpH_18Wrwq9O6mY_gHsCl6nTQm6IObcueZzBhQiN3bapOI3mBftGLsbAje5iQ662UpMeX3M43QUoTVsIfMIW5ttJMkouBCGWR70Bcp7fllx1wEL"/>
<span class="absolute top-3 right-3 px-3 py-1 rounded-full bg-white/90 backdrop-blur-sm text-primary text-[10px] font-extrabold uppercase">Sports</span>
</div>
<div class="p-md flex flex-col flex-1">
<h5 class="font-headline-md text-body-lg mb-1 group-hover:text-primary transition-colors">Super Soccer 2024</h5>
<p class="text-on-surface-variant text-sm line-clamp-2 mb-4">Le jeu de foot officiel du hub. Formez votre équipe et gagnez la coupe inter-lycées.</p>
<div class="mt-auto flex justify-between items-center">
<div class="flex -space-x-2">
<div class="w-6 h-6 rounded-full border-2 border-white bg-slate-200"><img alt="User" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDE0l1WGIeTuhkhxunh-b-EX--5301kYzBo017qMdkwk_LQa9-roLq_9KH6GEn2EWOshb-PIv_qqX1zMYBsvrJdCM_UPGmiJJLvKJbDciotzRFZyUQrAHLhQV7niGcYXu3eEoLU2EKL3Y6UCeDS2-VBkAd-8x_8Foret-y-iEjRLXl91kb5UrjkL0S4CdJAepD73BChJ6kx0D0JdM1_y7a14jO6gHw6Bu0C2LCL6hyCmyr2pSgqVEuJ6-lqgGy-Yg--GUn7k8q-Ufx6"/></div>
<div class="w-6 h-6 rounded-full border-2 border-white bg-slate-200"><img alt="User" src="https://lh3.googleusercontent.com/aida-public/AB6AXuBPRRp74QpKQuwMPhcXBShsEXy03Fn3-UaG5B4d-sxQ0FaWcPwsWSmv2DBO7tWBJWHx_ASxQsZfheEif9NVddAMpENTrk6Y0bvE7T6epIA2VF3uISAZpvEy6ZaQAC0pNC_QtBrQMwn13qVOa3z4Gtv-M9W_WxlUDO7r0DWqDgElpkNq0ag25_269XKF_XbKvsjYvBo3JolSPXzd9JM1rWWdvQB8c1s5i7ta5IXykthGPN-kubemSZraJd9iWdSYWL8pWxRhr2cAaSMy"/></div>
<div class="w-6 h-6 rounded-full border-2 border-white bg-slate-200 flex items-center justify-center text-[8px] font-bold">+12</div>
</div>
<button class="px-5 py-2 rounded-xl bg-primary-fixed text-on-primary-fixed-variant font-label-md hover:bg-primary transition-all hover:text-on-primary active:scale-95">Jouer</button>
</div>
</div>
</div>
<!-- Game Card 2 -->
<div class="bg-surface-container-lowest rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all group flex flex-col border border-outline-variant/30">
<div class="h-48 overflow-hidden relative">
<img class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" data-alt="A sophisticated digital landscape showing an abstract brain made of interconnected glowing nodes and circuitry in deep purple and magenta. The lighting is moody and focused, highlighting the intricate patterns. A clean, high-tempo aesthetic representing an advanced cognitive puzzle game for mature high schoolers." src="https://lh3.googleusercontent.com/aida-public/AB6AXuBRS9t_MmB7LZyPBKjLLabjLN2vpdPUnItff6VEbPK2O_N9SQSa8WPBSboj-aF1XYhMM_SMqzGn5bi8Hpgix9MblxcqF7JDbpXmd0Tb44ZI94hBbgTAG7I6TvJJekEmYLjsXPJUGvzIkjhuWm3L2UsTKhAWOtOQWh8b2iWtS17jNVUwAaCj96ZFcEi-AJR3vB3osEWZ-_RV3UOwlmIqHHqOSXZkUMSWd8Hxg6WRDBA9zIbMJvj8fxY3yxTBVNWvBFvJNCBVknqBa8le"/>
<span class="absolute top-3 right-3 px-3 py-1 rounded-full bg-white/90 backdrop-blur-sm text-tertiary text-[10px] font-extrabold uppercase">Puzzle</span>
</div>
<div class="p-md flex flex-col flex-1">
<h5 class="font-headline-md text-body-lg mb-1 group-hover:text-primary transition-colors">Neuro-Connect</h5>
<p class="text-on-surface-variant text-sm line-clamp-2 mb-4">Reliez les neurones le plus vite possible. Un défi mental pour les plus brillants.</p>
<div class="mt-auto flex justify-between items-center">
<span class="text-xs text-outline font-label-md italic">4.8 ★ (120 avis)</span>
<button class="px-5 py-2 rounded-xl bg-primary-fixed text-on-primary-fixed-variant font-label-md hover:bg-primary transition-all hover:text-on-primary active:scale-95">Jouer</button>
</div>
</div>
</div>
<!-- Game Card 3 -->
<div class="bg-surface-container-lowest rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all group flex flex-col border border-outline-variant/30">
<div class="h-48 overflow-hidden relative">
<img class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" data-alt="Dynamic 3D character art of a futuristic high school student hero in a sleek action pose. The style is inspired by modern animated films with vibrant cel-shading, rich textures, and dramatic lighting in shades of royal blue and gold. The atmosphere is heroic, optimistic, and high-tempo, perfect for an action-adventure game." src="https://lh3.googleusercontent.com/aida-public/AB6AXuBykyCR9VGs_8bgBIrhfZJaFl-QYQyjxO_NIPjq3KwTkVF3x3lfYxHV0eH5MhifE1h9iKubnE4X3byH_AKR-2JTTJd3VT53pGW9QgrG7y9APaZi3Kyb3C-uN8fb4SMJ9C_aqwnIHw0DKMwMGJ8CyFzLQ7iCXleoiwI2Rgtyj4Gd28UIYbmYVWWO-igl4BJBOOsPDQyNreoGhZhE1cQLYosu4TVLPHrE5X-gaYrxO0dNAoH17pZMb-FE4XXZGdIkVHcX9B01C8Ka0IbQ"/>
<span class="absolute top-3 right-3 px-3 py-1 rounded-full bg-white/90 backdrop-blur-sm text-secondary text-[10px] font-extrabold uppercase">Action</span>
</div>
<div class="p-md flex flex-col flex-1">
<h5 class="font-headline-md text-body-lg mb-1 group-hover:text-primary transition-colors">Hero Academy</h5>
<p class="text-on-surface-variant text-sm line-clamp-2 mb-4">Incarnez un super-héros au lycée. Missions, combats et pouvoirs épiques.</p>
<div class="mt-auto flex justify-between items-center">
<span class="text-xs text-outline font-label-md italic">Multijoueur</span>
<button class="px-5 py-2 rounded-xl bg-primary-fixed text-on-primary-fixed-variant font-label-md hover:bg-primary transition-all hover:text-on-primary active:scale-95">Jouer</button>
</div>
</div>
</div>
<!-- Game Card 4 -->
<div class="bg-surface-container-lowest rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition-all group flex flex-col border border-outline-variant/30">
<div class="h-48 overflow-hidden relative">
<img class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" data-alt="A vibrant digital chess board where the pieces are stylized as futuristic high-tech holograms in blue and purple. The scene is set in a modern, brightly lit study lounge with high-key lighting and a soft ambient glow. The aesthetic is sophisticated and intellectual, balancing strategy with high-end digital design." src="https://lh3.googleusercontent.com/aida-public/AB6AXuBmkU9Qm0renGuFcGOi64Wm-9KBEYT60C6F-CyQ8NlGKo1hswYO7ipp1vwqEMmcS-gltYZR5NmDNyzlYM5D4tn-Zg0us7G6urENUvzwic7JkMeRrPsA9VbcI4eegFLFKxhI6SHLX13gCAI-crOywG_2J4wbRl642JE__c0LqIqD5_ttXFBNbuNs7gDed0oUqEAlEn1jUA2efOAlKixMC6zRb_M-tGMR2hVTnwJ6kt9rVD_KheRGpsBKLI_KIVt-nZ2a0TBojtyHST3t"/>
<span class="absolute top-3 right-3 px-3 py-1 rounded-full bg-white/90 backdrop-blur-sm text-on-surface text-[10px] font-extrabold uppercase">Stratégie</span>
</div>
<div class="p-md flex flex-col flex-1">
<h5 class="font-headline-md text-body-lg mb-1 group-hover:text-primary transition-colors">Chess Hub 3000</h5>
<p class="text-on-surface-variant text-sm line-clamp-2 mb-4">Le jeu de stratégie classique avec des thèmes futuristes et des tournois.</p>
<div class="mt-auto flex justify-between items-center">
<span class="text-xs text-outline font-label-md italic">Nouveau</span>
<button class="px-5 py-2 rounded-xl bg-primary-fixed text-on-primary-fixed-variant font-label-md hover:bg-primary transition-all hover:text-on-primary active:scale-95">Jouer</button>
</div>
</div>
</div>
</div>
</section>
</main>
<!-- BottomNavBar -->
<nav class="fixed bottom-0 left-0 w-full h-20 flex justify-around items-center px-4 pb-safe bg-surface-container-low dark:bg-inverse-surface z-50 rounded-t-xl shadow-[0_-4px_24px_rgba(19,27,46,0.06)] dark:shadow-none">
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant hover:bg-surface-variant dark:hover:bg-on-surface-variant/10 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined" data-icon="grid_view">grid_view</span>
<span class="font-label-md text-label-md">Hub</span>
</a>
<a class="flex flex-col items-center justify-center bg-primary-container text-on-primary-container rounded-full px-4 py-1.5 transition-all active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined" data-icon="sports_esports" style="font-variation-settings: 'FILL' 1;">sports_esports</span>
<span class="font-label-md text-label-md">Games</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant hover:bg-surface-variant dark:hover:bg-on-surface-variant/10 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined" data-icon="article">article</span>
<span class="font-label-md text-label-md">News</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant hover:bg-surface-variant dark:hover:bg-on-surface-variant/10 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined" data-icon="star">star</span>
<span class="font-label-md text-label-md">Premium</span>
</a>
</nav>
<!-- Micro-interactions Script -->
<script>
        document.querySelectorAll('button, a').forEach(el => {
            el.addEventListener('click', (e) => {
                // Haptic feedback simulation
                if (window.navigator.vibrate) window.navigator.vibrate(10);
            });
        });

        // Search highlight effect
        const searchInput = document.querySelector('input[type="text"]');
        searchInput.addEventListener('focus', () => {
            searchInput.parentElement.classList.add('scale-[1.01]');
        });
        searchInput.addEventListener('blur', () => {
            searchInput.parentElement.classList.remove('scale-[1.01]');
        });
    </script>
</body></html>