## layout.tsx

```js
<html lang="en">
  <body className={inter.className}>
    <AppRouterCacheProvider>
      <ThemeProvider theme={darkTheme}>
        <CssBaseline />
        <Container>{children}</Container>
      </ThemeProvider>
    </AppRouterCacheProvider>
  </body>
</html>
```

## dark.theme.ts

```js
"use client";

import { createTheme } from "@mui/material";

const darkTheme = createTheme({
  palette: {
    mode: "dark",
  },
});

export default darkTheme;
```

## Center elements in the middle of the screen

```js
<Box className="h-screen flex items-center justify-center">{children}</Box>
```

## Make the Next.js Link have a Material UI styles

- import NextLink instead of Link from "next/link"
- NextLink is the alias of Link of "next/link", which means they are same
- so that then we can import Material UI Link now
