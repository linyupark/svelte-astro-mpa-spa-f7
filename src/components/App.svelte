<script>
  import { App, View } from "framework7-svelte";
  import routes from "./routes.js";

  const f7params = {
    // Array with app routes
    routes,
    // App Name
    name: "My App",
    // ...
  };
</script>

<App {...f7params}>
  <!-- initial page is specified in routes.js -->
  <View
    main
    browserHistory
    browserHistorySeparator=""
    browserHistoryInitialMatch={true}
    browserHistoryStoreHistory={false}
    url={location.href.replace(location.origin, "")}
    transition="f7-parallax"
    className="safe-areas"
    masterDetailBreakpoint={768}
  />
</App>
