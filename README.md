# Firebase Realtime Database Race Condition

This repository demonstrates a common race condition issue in Firebase Realtime Database applications using React. The problem occurs when reading and updating data asynchronously, causing inconsistent state updates.

## Problem

The `Counter` component retrieves and updates a counter value from the Firebase Realtime Database.  If multiple users or concurrent operations attempt to increment the counter, it is possible for the value to be overwritten or inconsistently updated, leading to incorrect counts.

## Solution

The solution involves using transactions or optimistic updates to ensure atomicity.  Transactions guarantee that updates are applied atomically, preventing race conditions. Optimistic updates provide a client-side solution that reduces server load.

## How to Reproduce

1. Clone the repository.
2. Install the required dependencies using npm install.
3. Configure your Firebase project and credentials.
4. Run the application.
5. Rapidly click the increment button to observe the race condition.

## License

MIT