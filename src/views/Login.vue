<template>
    <br><br><br><br><br>
    <div class="container-fluid mt-6">
      <div class="login-card p-4 rounded shadow-lg">
        <h2 class="text-center mb-4">Login</h2>
        <form @submit.prevent="handleLogin">
          <div class="mb-3">
            <label for="email" class="form-label">Email</label>
            <input
              type="email"
              class="form-control"
              id="email"
              v-model="email"
              placeholder="Nhập email"
              required
            />
          </div>
          <div class="mb-3">
            <label for="password" class="form-label">Mật Khẩu</label>
            <input
              type="password"
              class="form-control"
              id="password"
              v-model="password"
              placeholder="Nhập mật khẩu"
              required
            />
          </div>
          <button type="submit" class="btn btn-primary w-100">Đăng Nhập</button>
          <div class="text-center mt-3">
            <router-link to="/register" class="text-decoration-none">Không có tài khoản? Đăng Ký</router-link>
          </div>
        </form>
      </div>
    </div>
    <br><br><br><br><br>
  </template>
  
  <script>
  export default {
    name: 'Login',
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
  background: linear-gradient(to right, #ff7e5f, #feb47b); /* Đổi gradient nền */
  color: #fff;
}

.login-card {
  max-width: 4000px;
  width: 500px;
  background-color: #f9f9f9; /* Đổi nền thẻ login */
  color: #555; /* Đổi màu chữ */
  border-radius: 15px; /* Bo góc cho thẻ login */
  padding: 20px;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.1); /* Tạo bóng mờ cho thẻ */
}

.form-control {
  border-radius: 20px;
  border: 1px solid #ff7e5f; /* Đổi màu viền input */
}

.btn-primary {
  background-color: #ff7e5f; /* Đổi màu nền nút */
  border: none;
  border-radius: 20px;
  color: #fff;
}

h2 {
  color: #ff7e5f; /* Đổi màu chữ tiêu đề */
}

.btn-primary:hover {
  background-color: #feb47b; /* Đổi màu hover của nút */
}

.text-decoration-none {
  color: #ff7e5f; /* Đổi màu chữ liên kết */
}

.text-decoration-none:hover {
  text-decoration: underline;
  color: #feb47b; /* Đổi màu hover của liên kết */
}
</style>
