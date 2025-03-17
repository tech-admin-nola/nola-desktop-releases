# Release Notes  

# Ver 1.0.18
- Removed pending transaction completion flow due to a bug; it will be fixed later using the SITEF library directly.

- Added a new Debug flow with logging for WebSocket, polling, and other relevant app functionalities. All logs can now be monitored via CloudWatch.

- Removed the forced minimization to the Windows system tray, making the app stay visible on the taskbar for a more intuitive user experience.

- Added a reload button in Nola Desktop, positioned below the version field.

- Updated SITEF DLLs to version 104 (previously using version 90).

- Fixed PIX transactions for Nema and potentially Atelier stores.

- Stores not using REDE as an acquirer required a specific buffer input for PIX transactions.
   - The app was sending the incorrect automatic option for these stores.

- Fixed Pinpad communication issue