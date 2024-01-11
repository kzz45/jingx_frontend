<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
import { version, buildTime } from "../build/info.json";

console.log(
  `%cRelease Build Info 
%cVersion			v${version}
BuildTime		${buildTime}`,
  "background:#000;color:#FFF;font-weight:bold;",
  "background:#FFF;color:#000;"
);

export default {
  name: "App",
};
</script>
