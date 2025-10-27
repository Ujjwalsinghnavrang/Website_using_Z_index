# 🚀 CSS z-index Card Stack Project

This is a simple, single-page web project designed to demonstrate the functionality of the CSS `z-index` property. It features a stack of fanned-out image cards that interactively come to the front when hovered over.

## ✨ Features

* **Stacked Elements:** Cards are layered on top of each other using `position: absolute`.
* **Controlled Stacking:** The initial stacking order is explicitly set using `z-index` (from 1 to 4).
* **Interactive Hover Effect:** When a card (that isn't on top) is hovered over, its `z-index` is dynamically changed to `10`, bringing it in front of all other cards.
* **Visual Styling:** CSS `transform: rotate()` is used to "fan out" the cards for a more appealing visual presentation.

## 💻 Technologies Used

* **HTML5:** For the basic structure and content.
* **CSS3:** For all styling, positioning, and interaction logic.

## 💡 Key Concepts Demonstrated

This project is a great practical example of a few core CSS concepts:

1.  **Positioning Context:** The cards use `position: absolute` to allow them to overlap. This takes them out of the normal document flow.

2.  **`z-index`:** This property controls the stacking order of positioned elements.
    * `#card1` has `z-index: 4` (top)
    * `#card2` has `z-index: 3`
    * `#card3` has `z-index: 2`
    * `#card4` has `z-index: 1` (bottom)

3.  **`:hover` Pseudo-class:** This selector is used to change the `z-index` of a card when the mouse pointer is over it.
    ```css
    #card2:hover {
      z-index: 10;
    }
    
    #card3:hover {
      z-index: 10;
    }
    
    #card4:hover {
      z-index: 10;
    }
    ```
    Setting the `z-index` to `10` (a value higher than any other card's default `z-index`) ensures that the hovered card will always appear on top of the stack.

## 🚀 How to Run This Project

1.  **Clone the repository (or download the files):**
    ```sh
    git clone [your-repository-url]
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd [your-project-directory]
    ```
3.  **Open the `index.html` file:**
    Simply double-click the `index.html` file, or right-click and select "Open with" your preferred web browser.

That's it! You can now see the card stack and test the hover effect.
