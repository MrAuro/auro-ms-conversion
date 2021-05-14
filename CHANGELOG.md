# 1.2.0

-   Fixed bug where when the final result of a unit was 1 it would not be returned when using the short method:

    **Before:**

    ```js
    console.log(msConversion.relativeTime(137236834));
    // 14h, 7m, and 16s
    console.log(msConversion.relativeTime(137236834, true));
    // 1 day, 14 hours, 7 minutes, and 16 seconds
    ```

    **After:**

    ```js
    console.log(msConversion.relativeTime(137236834));
    // 1d, 14h, 7m, and 16s
    console.log(msConversion.relativeTime(137236834, true));
    // 1 day, 14 hours, 7 minutes, and 16 seconds
    ```

-   Removed index.d.ts
