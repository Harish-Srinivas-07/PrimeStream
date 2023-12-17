# 🎬 Prime Stream Web Application 🍿

Welcome to Prime Stream, a captivating web application designed for streaming movies and TV shows. Crafted with HTML, CSS, and JavaScript, Prime Stream fetches content dynamically from a CSV file on GitHub, ensuring real-time updates. Dive into different sections featuring Netflix Originals, Trending Now, All Time Favorites, New Arrivals, and Popular content.

## Features 🚀

- **Authentication:** Prime Stream leverages Azure AD B2C cloud for secure user authentication. Users must log in to access the exciting content.

- **Dynamic Content:** Movie data is sourced from a CSV file on GitHub, providing dynamic updates to the homepage based on various categories.

- **Responsive Design:** Enjoy a seamless user experience across devices with Prime Stream's responsive web design.

- **Persistent Storage:** Movie data is stored locally, enabling quick access and minimizing the need for frequent data fetching.

- **Popup Player:** Click the "Play" button to unveil a popup window with detailed information about the selected movie, including its trailer.

## Implementation ⚙️

### Authentication 🔐

1. Authentication is seamlessly handled via Azure AD B2C cloud. Users are directed to the authentication page (`https://primestreamer.netlify.app`) before accessing the main content.

2. Successful authentication is confirmed if the URL contains "code" or "id_token" parameters. Otherwise, users are prompted to log in.

### Movie Data 🎥

1. Movie data is dynamically fetched from a CSV file on GitHub. Categories include Netflix Originals, Trending Now, All Time Favorites, New Arrivals, and Popular.

2. The application checks local storage for existing movie data. If absent, it fetches the data from the CSV file, parsing and storing it locally.

### Movie Display 🍿

1. Movies are categorized and displayed in rows based on their category on the web page.

2. Clicking on a movie poster opens a popup window with comprehensive details about the movie, including the trailer.

### Popup Player 🎥

1. The popup window (`popup/index.html`) showcases essential movie details, allowing users to explore the title, year, duration, and description.

2. An embedded video player within the window facilitates smooth streaming of the movie trailer.

3. Users can interact with the movie details, toggling HD mode, expressing likes on Facebook, and initiating downloads.

## Usage 🌐

1. Explore the home page: [Prime Stream](https://primestream.netlify.app)

2. Authenticate using your Azure AD B2C account at [Prime Streamer](https://primestreamer.netlify.app).

3. Navigate through Netflix Originals, Trending Now, All Time Favorites, New Arrivals, and Popular content.

4. Click on a movie poster to unveil detailed information in the popup player.

5. Engage with the popup player by toggling HD mode, expressing likes on Facebook, and initiating downloads.

## How to Get Started 🚀

1. **Download Zip File:**
   - Visit [GitHub Repository](https://github.com/Harish-Srinivas-07/primestream).
   - Click on the "Code" button and select "Download ZIP."
   - Extract the downloaded ZIP file.

2. **Open in VS Code:**
   - Open the extracted folder in Visual Studio Code (VS Code).

3. **Run Index.html:**
   - In VS Code, open the integrated terminal.
   - Run the command `open index.html` or `start index.html`.
   - Alternatively, double-click the `index.html` file.

4. **User Credentials:**
   - Visit [Prime Streamer](https://primestreamer.netlify.app).
   - Create a user account to access Prime Stream.

## Video Streaming Provider 📺

Movies are available for download, stream, and like using [Streamtape](https://streamtape.com) as the video streaming provider.

## Disclaimer ⚠️

Hey streamers, use wisely to understand the frontend and backend implementation, dynamic updates of website content in a static website using CSV GitHub host, for educational purposes only.

**Lights, Camera, Action! Enjoy your streaming experience with Prime Stream! 🍿🎉**

## Bonus Note 🚨

🚫 **Developer Access:**
   - For developers, locate the script enforcing user redirection for account creation.
   - Remove the script to access Prime Stream without user credentials. ⚙️✨

## 📁 File Structure 🧐

The project follows the below file structure:

```plaintext
file :
->index.html
->style.css
->img folder:
          ->logo.png,icon.png,avatar.png,info.png
->popup folder:
           ->index.html,style.css
          -> img folder:
                    ->hd,like,back,logo.pngs
```
