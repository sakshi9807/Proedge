# Contacts Mobile App

This is a sample mobile app developed in React Native that displays the contacts of the phone and provides a search functionality. When a contact is clicked on, it shows the contact's name and number in a dismissable popup.

## Components

### App.js

This is the main component of the application. It utilizes the following components and libraries:

- `react`: The core library for building React applications.
- `react-native`: A library for building mobile applications using React.
- `react-native-contacts`: A library for accessing device contacts in React Native.
- `react-native-popup-dialog`: A library for creating popup dialogs in React Native.

#### State Variables

- `contacts`: An array that holds the phone's contacts retrieved from the device.
- `searchQuery`: A string that holds the current search query entered by the user.
- `selectedContact`: An object that represents the currently selected contact. It is set to `null` when no contact is selected.

#### useEffect Hook

- `loadContacts()`: A function called inside the `useEffect` hook to load the device's contacts using the `Contacts.getAll()` method and set them to the `contacts` state.

#### Event Handlers

- `handleContactPress(contact)`: An event handler called when a contact is pressed.
