<footer class="footer">
  <button class="menu-button">🏠</button>
  <button class="menu-button">🔍</button>
  <button class="menu-button active">👤</button>

  <style>
    .footer {
      display: flex;
      justify-content: space-around;
      align-items: center;
      padding: 10px 0;
      background-color: #fff;
      border-top: 1px solid #ddd;
    }

    .menu-button {
      background: none;
      border: none;
      font-size: 20px;
      cursor: pointer;
      color: #6c757d;
    }

    .menu-button.active {
      color: #007bff;
    }
  </style>
</footer>
