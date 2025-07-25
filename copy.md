<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ODIN - Sign Up</title>
    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

      body {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
          Oxygen, Ubuntu, Cantarell, sans-serif;
        min-height: 100vh;
        display: flex;
        background-color: #f9f9f9;
      }

      .left-panel {
        width: 35%;
        min-height: 100vh;
        background-image: url("https://images.unsplash.com/photo-1527004013197-933c4bb611b3?w=720");
        background-size: cover;
        background-position: center;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .left-panel::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0, 0.4);
      }

      .logo-banner {
        background-color: rgba(0, 0, 0, 0.6);
        width: 100%;
        padding: 20px 0;
        position: relative;
        z-index: 1;
        display: flex;
        align-items: center;
        justify-content: center;
        backdrop-filter: blur(5px);
      }

      .logo {
        display: flex;
        align-items: center;
        color: white;
        font-size: 3.5rem;
        font-weight: bold;
        letter-spacing: 0.1em;
      }

      .logo svg {
        width: 80px;
        height: 80px;
        margin-right: 10px;
      }

      .photo-credit {
        position: absolute;
        bottom: 10px;
        left: 50%;
        transform: translateX(-50%);
        color: white;
        font-size: 0.75rem;
        z-index: 1;
      }

      .photo-credit a {
        color: white;
        text-decoration: underline;
      }

      .right-panel {
        width: 65%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding: 0 40px;
        background-color: #f9f9f9;
      }

      .intro-text {
        max-width: 600px;
        margin-bottom: 40px;
      }

      .intro-text p {
        font-size: 1.25rem;
        font-weight: 600;
        margin-bottom: 20px;
        color: #333;
        line-height: 1.4;
      }

      .intro-text .emphasis {
        font-style: italic;
        font-weight: 500;
      }

      .intro-text .know {
        font-style: italic;
      }

      .form-section {
        background-color: white;
        padding: 40px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        margin: 0 -40px;
        position: relative;
      }

      .form-section h2 {
        font-size: 1.5rem;
        margin-bottom: 30px;
        color: #333;
      }

      .form-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 20px 30px;
        max-width: 600px;
      }

      .form-group {
        display: flex;
        flex-direction: column;
      }

      .form-group label {
        font-size: 0.75rem;
        font-weight: 600;
        letter-spacing: 0.1em;
        text-transform: uppercase;
        color: #555;
        margin-bottom: 5px;
      }

      .form-group input {
        padding: 8px 10px;
        border: 1px solid #e5e5e5;
        border-radius: 4px;
        font-size: 1rem;
        transition: border-color 0.3s;
      }

      .form-group input:focus {
        outline: none;
        border-color: #4a6741;
        box-shadow: 0 0 0 3px rgba(74, 103, 65, 0.1);
      }

      .submit-section {
        padding: 30px 40px;
        max-width: 600px;
      }

      .submit-btn {
        background-color: #596d48;
        color: white;
        border: none;
        padding: 15px 50px;
        font-size: 1rem;
        font-weight: 600;
        border-radius: 8px;
        cursor: pointer;
        transition: all 0.3s;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      }

      .submit-btn:hover {
        background-color: #4a5a3a;
        transform: translateY(-2px);
        box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
      }

      .login-link {
        margin-top: 30px;
        font-size: 1rem;
        color: #333;
      }

      .login-link a {
        color: #596d48;
        text-decoration: none;
        font-weight: 600;
      }

      .login-link a:hover {
        text-decoration: underline;
      }

      @media (max-width: 768px) {
        body {
          flex-direction: column;
        }

        .left-panel,
        .right-panel {
          width: 100%;
        }

        .left-panel {
          min-height: 30vh;
        }

        .form-grid {
          grid-template-columns: 1fr;
        }

        .form-section {
          margin: 0;
          padding: 20px;
        }

        .submit-section {
          padding: 20px;
        }
      }
    </style>
  </head>
  <body>
    <div class="left-panel">
      <div class="logo-banner">
        <div class="logo">
          <svg
            viewBox="0 0 100 100"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M50 10L80 30V50L70 90H30L20 50V30L50 10Z"
              stroke="white"
              stroke-width="3"
              fill="none"
            />
            <path
              d="M50 10L50 40M50 40L30 50M50 40L70 50"
              stroke="white"
              stroke-width="3"
            />
            <circle cx="40" cy="55" r="3" fill="white" />
            <circle cx="60" cy="55" r="3" fill="white" />
            <path
              d="M35 70Q50 80 65 70"
              stroke="white"
              stroke-width="3"
              fill="none"
            />
          </svg>
          ODIN
        </div>
      </div>
      <div class="photo-credit">
        Photo by <a href="#">Halie West</a> on <a href="#">Unsplash</a>
      </div>
    </div>

    <div class="right-panel">
      <div class="intro-text">
        <p>
          This is not a real online service! You know you need something like
          this in your life to help you realize your deepest dreams.
        </p>
        <p>Sign up <span class="emphasis">now</span> to get started.</p>
        <p class="know">You <span class="know">know</span> you want to.</p>
      </div>

      <form>
        <div class="form-section">
          <h2>Let's do this!</h2>
          <div class="form-grid">
            <div class="form-group">
              <label for="first-name">FIRST NAME</label>
              <input
                type="text"
                id="first-name"
                name="firstName"
                value="Thor"
                required
              />
            </div>
            <div class="form-group">
              <label for="last-name">LAST NAME</label>
              <input
                type="text"
                id="last-name"
                name="lastName"
                value="Odinson"
                required
              />
            </div>
            <div class="form-group">
              <label for="email">EMAIL</label>
              <input type="email" id="email" name="email" required />
            </div>
            <div class="form-group">
              <label for="phone">PHONE NUMBER</label>
              <input type="tel" id="phone" name="phone" />
            </div>
            <div class="form-group">
              <label for="password">PASSWORD</label>
              <input type="password" id="password" name="password" required />
            </div>
            <div class="form-group">
              <label for="confirm-password">CONFIRM PASSWORD</label>
              <input
                type="password"
                id="confirm-password"
                name="confirmPassword"
                required
              />
            </div>
          </div>
        </div>

        <div class="submit-section">
          <button type="submit" class="submit-btn">Create Account</button>
          <div class="login-link">
            Already have an account? <a href="#">Log in</a>
          </div>
        </div>
      </form>
    </div>
  </body>
</html>
