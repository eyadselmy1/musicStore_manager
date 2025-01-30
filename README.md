# Music Store Management System

## Overview

This Music Store Management System is a Python-based application designed to help store managers efficiently manage the rental of music records. The system allows for the searching, renting, returning, and inventory management of CDs, vinyl, and cassette tapes based on customer subscriptions.

## Features:

### Customer Management

Customers are identified by unique four-letter IDs (e.g., "coab").

Only customers with active subscriptions (validated via subscriptionManager.pyc) can rent music records.

### Music Inventory Management

Stores and manages details of music records, including:

- Artist

- Title

- Medium (CD, Vinyl, Tape)

- Genre (e.g., Pop, Classical, Jazz, Hip Hop, Rap, Kwaito)

- Purchase Date

- Unique ID number

Maintains a rental history log for each music record.

### Search Functionality

Allows store managers to search for music by:

- Artist

- Title

- Medium

- Genre

Displays search results with availability status.

### Music Renting Functionality

Managers can rent out music records by providing a customer ID and the music record’s unique ID.

The system validates input and checks:

- If the customer has an active subscription.

- If the music record is available for rent.

- If the customer has reached their rental limit.

Provides appropriate success or error messages based on rental status.

### Returning Music Records & Collecting Feedback Functionality

Store managers can log the return of a music record by entering its unique ID.

Customers can provide a star rating and optional comments.

Feedback is stored in an external database via feedbackManager.pyc.

### Inventory Pruning Functionality

Identifies unpopular music records based on rental frequency.

Provides suggestions for optimizing inventory by removing underutilized records.

Includes visualization tool for better decision-making.

### Technologies Used

Programming Language: Python (Standard Libraries, Matplotlib & NumPy)

Development Environment: JupyterLab (.ipynb Notebook)

Database: Plain text files (Music_Info.txt, Rental.txt, etc.)

GUI Framework: iPyWidgets (for interactive menu)

External Modules: subscriptionManager.pyc (Manages customer subscriptions), feedbackManager.pyc (Handles customer feedback collection)
