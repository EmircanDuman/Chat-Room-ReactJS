# Chat-Room-ReactJS
a chat room application that uses Firebase API
You'll need to create and manage a Firebase backend to use it.
Or rather just follow along this tutorial:
https://www.youtube.com/watch?v=0gLr-pBIPhI&list=WL&index=6&ab_channel=PedroTech

Create a firebase-config.js in the main src folder,

import { initializeApp } from "firebase/app";
import { getAuth, GoogleAuthProvider } from 'firebase/auth';
import { getFirestore } from '@firebase/firestore';


fill in your firebase firebase config code here*

// Initialize Firebase
const app = initializeApp(firebaseConfig);

export const auth = getAuth(app);
export const provider = new GoogleAuthProvider();
export const db = getFirestore(app);
