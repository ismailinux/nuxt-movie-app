<template>
    <footer class=" py-8 text-gray-500 text-left mt-6">
      <p class="text-sm md:text-base">&copy; {{ new Date().getFullYear() }} Opaluwa Ismail. All rights reserved. 
      </p>
      <p class="text-sm md:text-base mt-2">Designed and built by me, data provided by 
        <a class="underline" target="_blank" href="https://www.themoviedb.org/" rel="noopener">TMDb</a>.
      </p>
  
      <ul class="flex mt-2">
        <li v-for="link in socialLinks" :key="link.href" class="">
          <a 
            :href="link.href" 
            target="_blank" 
            :aria-label="link.label" 
            rel="noopener" 
            class="flex items-center w-11 h-11 transition-all duration-300 ease-in-out hover:text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" :fill="link.color">
              <path :d="link.path" />
            </svg>
          </a>
        </li>
      </ul>
    </footer>
  </template>
  
  <script>
  export default {
    data() {
      return {
        socialLinks: [
          {
            href: "https://x.com/MonsieurFemi",
            label: "Link to Twitter account",
            color: "#585858",
            path: "M12.6.75h2.454l-5.36 6.142L16 15.25h-4.937l-3.867-5.07-4.425 5.07H.316l5.733-6.57L0 .75h5.063l3.495 4.633L12.601.75Zm-.86 13.028h1.36L4.323 2.145H2.865z",
          },
          {
            href: "https://github.com/ismailinux",
            label: "Link to GitHub account",
            color: "#585858",
            path: "M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8",
          },
          {
            href: "https://www.linkedin.com/in/ismail-opaluwa-74a016236/",
            label: "Link to LinkedIn account",
            color: "#585858",
            path: "M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z",
          },
          {
            href: "mailto:ismailenox@gmail.com",
            label: "Link to Email",
            color: "#585858",
            path: "M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2zm2-1a1 1 0 0 0-1 1v.217l7 4.2 7-4.2V4a1 1 0 0 0-1-1zm13 2.383-4.708 2.825L15 11.105zm-.034 6.876-5.64-3.471L8 9.583l-1.326-.795-5.64 3.47A1 1 0 0 0 2 13h12a1 1 0 0 0 .966-.741M1 11.105l4.708-2.897L1 5.383z",
          },
        ],
      };
    },
  };
  </script>
  