# Red-Black Tree Visualization

This is an interactive web application designed to visualize the structure and operations of a Red-Black Tree, a type of self-balancing binary search tree. It provides a visual aid for understanding how insertions and deletions maintain the tree's balance properties through rotations and color changes.


## Features

*   **Interactive Visualization:** View the Red-Black Tree structure graphically using SVG.
*   **Node Insertion:** Insert new nodes with integer values (1-999). The visualization updates dynamically, showing balancing operations if necessary.
*   **Node Deletion:** Delete existing nodes by value. The visualization updates to reflect the removal and subsequent rebalancing.
*   **Reset Tree:** Clear the current tree and start fresh.
*   **Generate Random Tree:** Create a random Red-Black Tree with 5-15 nodes for quick experimentation.
*   **Pan & Zoom:**
    *   Click and drag on the visualization area to pan the view.
    *   Use the '+' and '-' buttons to zoom in and out.
    *   Use the "Reset View" button to restore the default pan and zoom levels.
*   **Dark Mode:** Automatically adapts to your system's preferred color scheme (light or dark).
*   **Property Display:** Shows the fundamental properties of Red-Black Trees for reference.
*   **Status Messages:** Provides feedback on operations (e.g., "Inserted 50", "Value 25 not found").

## How to Use

1.  **Download:** Save the `index.html` (or rename the provided HTML file to `index.html`) file to your local machine.
2.  **Open:** Double-click the `index.html` file to open it in your preferred web browser (e.g., Chrome, Firefox, Safari, Edge).
    *   **Note:** An internet connection is required on the first load (or when cache is cleared) to fetch the Tailwind CSS framework from the CDN.
3.  **Interact:** Use the controls described below to build and manipulate the Red-Black Tree.

## Controls

Located in the top-left panel:

*   **Insert Node:**
    *   Enter an integer value (1-999) into the input field.
    *   Click the "Insert" button or press Enter.
*   **Delete Node:**
    *   Enter the integer value of the node you wish to delete.
    *   Click the "Delete" button or press Enter.
*   **Reset Tree:** Click this button to remove all nodes from the tree.
*   **Generate Random Tree:** Click this button to clear the current tree and generate a new one with random values.
*   **Status Area:** Displays messages about the last operation performed.

## Visualization Area

Located in the top-right panel:

*   **Canvas:** The main area where the Red-Black Tree is drawn using SVG.
    *   Red nodes are represented by red circles.
    *   Black nodes are represented by black (or dark gray in dark mode) circles.
    *   Edges connect parent nodes to their children.
*   **Panning:** Click and drag within the canvas area to move the tree view.
*   **Zoom Buttons:**
    *   `+`: Zoom In
    *   `-`: Zoom Out
*   **Reset View Button:** Resets the pan and zoom to the default state without affecting the tree itself.

## Red-Black Tree Properties

Located in the bottom panel, this section lists the defining rules of a Red-Black Tree:

1.  Every node is either red or black.
2.  The root is black.
3.  All leaves (NIL nodes, conceptually) are black.
4.  If a node is red, then both its children are black (no two red nodes in a row on any path).
5.  Every path from a given node to any of its descendant NIL nodes contains the same number of black nodes (the "black-height" property).

It also mentions the balancing operations (color changes, left/right rotations) used to maintain these properties.

## Technology Stack

*   **HTML:** Structure of the web page.
*   **CSS (Tailwind CSS):** Styling and layout (via CDN).
*   **JavaScript:**
    *   Red-Black Tree data structure implementation (Node and RedBlackTree classes).
    *   SVG manipulation for visualization (TreeVisualizer class).
    *   DOM manipulation and event handling for user interaction.
*   **SVG (Scalable Vector Graphics):** Used to draw the tree visualization.

## License

This project is provided as-is. You are free to use, modify, and distribute it.