## P2P File Transfer Chat

A minimalist and serverless Peer-to-Peer (P2P) file transfer and chat application built with **WebRTC**. 
Transfer files and messages directly between browsers without any intermediate server storage.

----------

### Features

-   **Direct P2P Transfer:** Files and messages travel directly from browser to browser using WebRTC.
    
-   **Handshake Protocol:** Secure file transfers! The receiver must manually **Accept** or **Deny** any incoming file request.
    
-   **Privacy First:** No server ever sees or stores your data. PeerJS is used only for the initial signaling.
    
-   **Transfer Confirmation:** Visual feedback when a file is successfully sent and received.
    
-   **Dark Mode Support:** Toggle between light and dark themes with persistent storage.
    
-   **Responsive Design:** Fully optimized for mobile and desktop browsers.
    
-   **Connection Management:** Stable connection with automatic reconnect and manual disconnect options.
    

### How to Use

1.  **Open the App:** Both users open the application in their respective browsers.
    
2.  **Share ID:** Copy your unique **ID** by clicking on it and share it with your partner (via email, messenger, etc.) or use share Link.
    
3.  **Connect:** Enter your partner's ID into the input field and click the **Connect** icon.
    
4.  **Chat & Send:** Once the status turns green (**Connected**), you can chat or click the **Paperclip** icon to send files (Max 50MB).
    
5.  **Confirm:** The receiver will see a request to accept the file before the transfer begins.
    

### Built With

-   **PeerJS** - WebRTC wrapper for easy P2P signaling.
    
-   **Lucide Icons** - Beautiful and consistent iconography.
    
-   **Pure HTML/CSS/JS** - No complex frameworks, ensuring maximum performance.
    

### Security & Technical Details

-   **Data Security:** Data is encrypted via the browser's native WebRTC implementation.
    
-   **Signaling:** We use the public PeerJS signaling server to help peers find each other. 
Once connected, the server is no longer involved in the data flow.
    
-   **File Limits:** For stability, transfers are limited to **50MB**. 
This prevents browser memory (RAM) crashes, as WebRTC data is currently buffered in memory.
    
-   **Handshake:** The custom handshake ensures you never receive unwanted files.

    

### License
MIT

### Live Demo Link:
https://bmpydev.github.io/p2p-file-transfer-chat/
