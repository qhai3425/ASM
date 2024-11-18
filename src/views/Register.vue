<template>
    <br><br><br><br><br>
    <div class="container-fluid mt-6">
      <div class="login-card p-4 rounded shadow-lg">
        <h2 class="text-center mb-4">Đăng Kí</h2>
        <form >
          <div class="mb-3">
            <label for="email" class="form-label">Email</label>
            <input
              type="email"
              class="form-control"
              id="email"
              placeholder="Nhập email"
              required
            />
          </div>
          <div class="mb-3">
            <label for="email" class="form-label">Tên</label>
            <input
              type="email"
              class="form-control"
              id="email"
              placeholder="Nhập Tên"
              required
            />
          </div>
          <div class="mb-3">
            <label for="password" class="form-label">Mật Khẩu</label>
            <input
              type="password"
              class="form-control"
              id="password"
              placeholder="Nhập mật khẩu"
              required
            />
          </div>
          <button type="submit" class="btn btn-primary w-100">Đăng Kí</button>
          <div class="text-center mt-3">
            <router-link to="/login" class="text-decoration-none">Đã có tài khoản</router-link>
          </div>
        </form>
      </div>
    </div>
    <br><br><br><br><br>
  </template>
  
  <script>
  export default {
    name: 'register',
    data() {
      return {
        email: '',
        password: '',
      };
    },
    methods: {
      handleLogin() {
        if (this.email && this.password) {
          alert(`Logged in with Email: ${this.email}`);
        } else {
          alert('Please fill in all fields.');
        }
      },
    },
  };
  </script>
  
  <style scoped>
  .navbar {
    left: 0;
    width: 100%;
  }
  
  .login-page {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh; /* Căn giữa theo chiều dọc */
    background: linear-gradient(to right, #ff7e5f, #feb47b); /* Màu nền gradient */
    color: #fff;
  }
  
  .login-card {
    max-width: 4000px;
    width: 800px;
    background-color: #fff;
    color: #333;
    border-radius: 15px; /* Bo góc cho thẻ login */
    padding: 20px;
    box-shadow: 0 0 15px rgba(0, 0, 0, 0.1); /* Tạo bóng mờ cho thẻ */
  }
  
  .form-control {
    border-radius: 20px;
  }
  
  .btn-primary {
    border-radius: 20px;
    background-color: #ff7e5f;
    border-color: #ff7e5f;
  }
  
  .btn-primary:hover {
    background-color: #feb47b;
    border-color: #feb47b;
  }
  
  h2 {
    color: #ff7e5f; /* Màu tiêu đề */
  }
  
  .text-decoration-none {
    color: #ff7e5f; /* Màu liên kết */
  }
  
  .text-decoration-none:hover {
    text-decoration: underline;
    color: #feb47b; /* Màu liên kết khi hover */
  }
  </style>
  