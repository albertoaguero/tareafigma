<script>
    export let user;
  </script>
  
  <section class="profile">
    <div class="avatar">
      <img src={user.avatar} alt="Avatar de usuario" />
      <button class="edit-avatar">✏️</button>
    </div>
    <h2>{user.name}</h2>
    <p>{user.username}</p>
  
    <style>
      .profile {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 20px;
        background-color: #fff;
        border-bottom: 1px solid #ddd;
      }
  
      .avatar {
        position: relative;
        margin-bottom: 10px;
      }
  
      .avatar img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 2px solid #ddd;
      }
  
      .edit-avatar {
        position: absolute;
        bottom: 0;
        right: 0;
        background: #007bff;
        color: #fff;
        border: none;
        border-radius: 50%;
        font-size: 14px;
        cursor: pointer;
        padding: 5px;
      }
    </style>
  </section>
  