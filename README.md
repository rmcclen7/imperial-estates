// File: RealEstateWidgets.tsx (or .jsx if JS only)

import * as React from "react";

export function RealEstateWidgets() {
  return (
    <iframe
      src="https://imperialistings.github.io/widgets.html" // Replace with your real URL
      width="100%"
      height="1200"
      style={{
        border: "none",
        background: "transparent",
        overflow: "hidden",
      }}
      loading="lazy"
      allowFullScreen
    />
  );
}
