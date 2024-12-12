<script>
    export let user;
  </script>
  
  <section class="options">
    {#each user.options as option}
      <div class="option">
        <span class="icon">{option.icon}</span>
        <span class="name">{option.name}</span>
        <span class="arrow">➡️</span>
      </div>
    {/each}
  
    <style>
      .options {
        flex: 1;
        display: flex;
        flex-direction: column;
        background-color: #f8f9fa;
      }
  
      .option {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 15px 20px;
        border-bottom: 1px solid #ddd;
        cursor: pointer;
        transition: background-color 0.2s;
      }
  
      .option:hover {
        background-color: #e9ecef;
      }
  
      .icon {
        font-size: 20px;
        margin-right: 10px;
      }
  
      .name {
        flex: 1;
      }
  
      .arrow {
        font-size: 18px;
        color: #6c757d;
      }
    </style>
  </section>
  