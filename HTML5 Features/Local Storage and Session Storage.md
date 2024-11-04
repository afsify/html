# Web Storage API

The Web Storage API provides a way to store key/value pairs in a web browser, allowing for the storage of data on the client-side. It includes two primary storage types: **Local Storage** and **Session Storage**.

#### 1. Local Storage

**Local Storage** is designed for storing data that needs to persist even after the browser window is closed. It is domain-specific and can store up to 5-10 MB of data (varies by browser).

- **Characteristics**:
  - Data persists across sessions (i.e., it remains available after the browser is closed and reopened).
  - Data is stored as key/value pairs.
  - Synchronous API (data is accessed immediately).
  - Limited storage capacity (generally between 5-10 MB).
  - Data is accessible within the same origin (same domain and protocol).

- **Usage**:
  - Set an item: `localStorage.setItem(key, value)`
  - Get an item: `localStorage.getItem(key)`
  - Remove an item: `localStorage.removeItem(key)`
  - Clear all items: `localStorage.clear()`
  - Check the length of items: `localStorage.length`
  
- **Example**:
    ```javascript
    // Storing data
    localStorage.setItem('username', 'JohnDoe');
    
    // Retrieving data
    const username = localStorage.getItem('username');
    console.log(username); // Output: JohnDoe
    
    // Removing data
    localStorage.removeItem('username');
    
    // Clearing all data
    localStorage.clear();
    ```

#### 2. Session Storage

**Session Storage** is intended for storing data for a single session. It is cleared when the page session ends (i.e., when the tab or window is closed).

- **Characteristics**:
  - Data persists only within the current browser tab/window.
  - Data is stored as key/value pairs.
  - Synchronous API.
  - Limited storage capacity (typically the same as local storage).
  - Data is accessible only within the same session (same tab/window).

- **Usage**:
  - Set an item: `sessionStorage.setItem(key, value)`
  - Get an item: `sessionStorage.getItem(key)`
  - Remove an item: `sessionStorage.removeItem(key)`
  - Clear all items: `sessionStorage.clear()`
  - Check the length of items: `sessionStorage.length`

- **Example**:
    ```javascript
    // Storing data
    sessionStorage.setItem('sessionID', '12345ABC');
    
    // Retrieving data
    const sessionID = sessionStorage.getItem('sessionID');
    console.log(sessionID); // Output: 12345ABC
    
    // Removing data
    sessionStorage.removeItem('sessionID');
    
    // Clearing all data
    sessionStorage.clear();
    ```

#### 3. Differences Between Local Storage and Session Storage

| Feature                     | Local Storage                           | Session Storage                       |
|-----------------------------|----------------------------------------|--------------------------------------|
| Data Persistence             | Persists until explicitly deleted      | Persists only during a session       |
| Scope                       | Available across all tabs/windows      | Available only in the current tab    |
| Capacity                    | Typically 5-10 MB per domain          | Typically 5-10 MB per tab            |
| Use Case                    | Storing user preferences, themes, etc. | Storing temporary data for a session |

#### 4. Common Use Cases

- **Local Storage**:
  - Storing user preferences (e.g., theme settings).
  - Caching data (e.g., user authentication tokens).
  - Persisting shopping cart items across sessions.

- **Session Storage**:
  - Storing data that only needs to last for a single session (e.g., form input data).
  - Temporary caching of user state while navigating through a multi-step process.

#### 5. Limitations

- Data is stored as strings. To store objects, you need to serialize them using `JSON.stringify()` and deserialize with `JSON.parse()`.
- The size limit can vary by browser and is generally around 5-10 MB per origin.
- Data stored in local storage and session storage is not secure and should not be used for sensitive information (e.g., passwords).

### Summary

The Web Storage API provides a powerful way to store data in web applications using Local Storage and Session Storage. Local Storage is ideal for persisting data across sessions, while Session Storage is suited for temporary data that only needs to last for a single session. Understanding the differences and use cases for each can help you effectively manage client-side storage in your web applications.