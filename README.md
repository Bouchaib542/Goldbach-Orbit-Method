# Goldbach Orbit Method

A fast JavaScript implementation of the Goldbach Orbit Method using √E-guided search and orbital classification to find prime pairs (p, q) such that p + q = E, even for E ≥ 10¹⁹.

## 🔍 Description
This program predicts and finds Goldbach pairs (p, q) for a given even number E by scanning symmetrically around E/2.  
The search is dynamically guided by the theoretical bound:

δ(E) ≈ √E · (log log E) / log E

Three orbit layers are used:
- **Central orbit**: p ≈ E/2
- **Orbital layer**: |p − E/2| ≤ δ(E)
- **Peripheral region**: beyond δ(E)

The algorithm avoids browser crashes by using a progressive batch search (1000 steps per cycle) and handles extremely large even numbers efficiently.

## ✅ Features
- Handles even numbers up to **10¹⁹ and beyond**
- Classifies results by **orbital layer**
- Written in **pure JavaScript** (BigInt)
- Works on **desktop and mobile browsers**
- Deployable on **GitHub Pages**

## 🚀 How to Use
1. Clone or download this repository.
2. Open `index.html` in any modern browser.
3. Enter a large even number (e.g., `10000000000000000000`)
4. Click **Find Goldbach Pair**
5. View the result with orbit layer classification.

## 🌐 Live Demo
Once deployed via GitHub Pages:

https://<your-username>.github.io/Goldbach-Orbit-Method/

## 👨‍🔬 Author
Bahbouhi Bouchaib — Independent researcher, Nantes, France.

## 📜 License
This method and code are public and free to use.
