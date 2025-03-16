# Project Workshop with JavaFX and JDBC

## Table of Contents

1. [General Objective](#general-objective)
2. [Technologies Used](#technologies-used)
3. [Project Overview](#project-overview)
	1. [JavaFX MVC](#javafx-mvc)
	2. [Views](#views)
4. [Versions](#versions)
5. [Tools](#tools-macos)
	1. [Scene Builder](#scene-builder)
	2. [Eclipse](#eclipse)
	3. [JavaFX SDK](#javafx-sdk)
	4. [MySQL Connector](#mysql-connector)
6. [Configure the Tools](#configure-the-tools-macos)

---

## General Objective

- Learn JavaFX application development with JDBC.

- Know the fundamentals and use of tools.

- Use Scene Builder to speed up creating JavaFX UIs.

---

## Technologies Used

### JavaFX

- JavaFX is a multimedia software platform developed by Sun Microsystems based on Java for creating and delivering Rich Internet Application that can run on many different devices.

### Scene Builder

- Scene Builder is a visual layout tool that lets users quickly design JavaFX application user interfaces, without coding. Users can drag and drop UI components to a work area, modify their properties, apply style sheets, and the FXML code for the layout that they are creating is automatically generated in the background.

---

## Project Overview

- The project consists of an application that handles information from sellers and departments in a workshop.

### JavaFX MVC

- JavaFX is designed based on the MVC pattern
- The Model - consists of the domain data and all logic for transforming this data
- The Views - These are the user interaction (UI) screens
- Controllers – These are the classes responsible for handling user interactions with views (handling interaction events with screens)

<img src="/src/assets/imgs/model_mvc.png" alt="MVC" style="width: 600px;">

### Views

#### Home Screen

<img src="/src/assets/imgs/home.png" alt="Home Screen" style="width: 600px;">

#### Tool Bar Options

##### Registration Option

<img src="/src/assets/imgs/home_option_1.png" alt="Home Option" style="width: 600px;">

##### Help Option

<img src="/src/assets/imgs/home_option_2.png" alt="Home Option" style="width: 600px;">

#### About Screen

<img src="/src/assets/imgs/about.png" alt="About" style="width: 600px;">

#### Seller Screen

<img src="/src/assets/imgs/seller.png" alt="Seller Screen" style="width: 600px;">

#### Enter Seller

<img src="/src/assets/imgs/seller_enter.png" alt="Enter Seller" style="width: 600px;">

#### Enter Department

<img src="/src/assets/imgs/department_enter.png" alt="Enter Department" style="width: 600px;">

#### Delete Screen

<img src="/src/assets/imgs/delete.png" alt="Delete Screen" style="width: 600px;">

---

## Versions

- Java 21.0.3
- MySQL Java Connector 8.4.0
- JavaFX 17.0.11

---

## Tools (MacOS)

### Scene Builder

- Download [Scene Builder](https://gluonhq.com/products/scene-builder/)

### Eclipse

- Download [Eclipse](http://www.eclipse.org/downloads/packages/)

### JavaFX SDK

- Download [JavaFX SDK](https://gluonhq.com/products/javafx)

### MySQL Connector

- Download [MySQL Connector](https://dev.mysql.com/downloads/connector/j/) - Select **Platform Independent**

---

## Configure the Tools (MacOS)

### Eclipse

1. Install the E(fx)clipse plug-in:
	- Help -> Install new Software
	- Work with: `http://download.eclipse.org/efxclipse/updates-released/3.4.1/site/`
	- Select all options and restart Eclipse
	
2. Reference SceneBuilder in Eclipse:
	- Window -> Preferences -> JavaFX
	- Put the SceneBuilder.app as executable

3. Create a User Library in Eclipse named JavaFX and other named MySQLConnector:
	- Window -> Preference -> Java -> Build Path -> User Libraries -> New
	- Add External Jars (Select .jar files from the libraries you downloaded)
	
4. Configure the build:
	- Before you run the project for the first time:
    - At the project folder: Run As -> Run Configurations -> VM Arguments
    - Copy that to the there, adapting to your JavaFX SDK folder:
    - `--module-path "C:\java-libs\javafx-sdk\lib" --add-modules=javafx.fxml,javafx.controls`
    - Dismark this option: `Use the -XstartOnFirstThread argument when launching with SWT`
	 
