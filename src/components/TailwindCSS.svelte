<script>
  const currentTheme = typeof window !== 'undefined' ? localStorage.getItem("theme") : null;
  if (currentTheme) {
    document.documentElement.setAttribute("data-theme", currentTheme);
  } else {
    typeof window !== 'undefined' && window.matchMedia("(prefers-color-scheme: dark)").addListener(e => {
        if (e.matches) {
            document.documentElement.setAttribute("data-theme", "dark")
        } else {
            document.documentElement.setAttribute("data-theme", "light")
        }
    });
  }
</script>

<style global>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;


  /* [data-theme="dark"] {
    --text-color: white;
    --bg-color: #212121;
  }
  [data-theme="dark"] .icon {
    filter: invert(100%);
    color: #212121;
  }
  [data-theme="sepia"] {
    --text-color: #402b0c;
    --bg-color: #eae0b9;
  }
  [data-theme="sepia"] .card {
    border-color: var(--text-color);
  }
  [data-theme="sepia"] .text-gray-500 {
    color: #896f47;
  }
  [data-theme="sepia"] .placeholder-gray-500::placeholder {
    color: #896f47;
  }
  [data-theme="sepia"] .text-gray-600 {
    color: #5e4828;
  }
  [data-theme="sepia"] .border-gray-300 {
    border-color: #a8906b;
  }
  [data-theme="sepia"] .border-gray-600 {
    border-color: #5e4828;
  }
  [data-theme="sepia"] .bg-gray-200 {
    background-color: #d8c3a2;
  } */
</style>