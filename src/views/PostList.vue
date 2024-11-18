<template>
    <br><br><br>
  <!-- Container wrapper -->
    <!-- Navbar brand -->
    
 <div class="container-fluid">
         <h2>Trang Post</h2>
         <p>Danh sách blog<br></p>
       </div><!-- End Section Title -->
 

           <div class="col-lg-12 col-md-12 col-sm-12" >
             <article>
 
               <div class="post-img">
                 <img :src="imageUrl2" alt="" class="img-fluid">
               </div>
 
               <p class="post-category">Sports</p>
 
               <h2 class="title">
                 <a href="http://localhost:5173/postsdetail">Thám tử lừng danh Conan | Tập 212: Vụ án giết người trong phòng kín</a> <button class="btn btn-outline-primary">Like</button> |
                 <button class="btn btn-outline-success">Share </button>
               </h2>
 
               <div class="d-flex align-items-center">
                 <img src="" alt="" class="img-fluid post-author-img flex-shrink-0">
                 <div class="post-meta">
                   <p class="post-author">Allisa Mayer</p>
                   <p class="post-date">
                     <time datetime="2022-01-01">Jun 5, 2022</time>
                   </p>
                 </div>
               </div>
 
             </article>
           </div><!-- End post list item -->
           <br><br>

           <div class="col-lg-12 col-md-12 col-sm-12" data-aos-delay="300">
             <article>
 
               <div class="post-img">
                 <img :src="imageUrl3" alt="" class="img-fluid">
               </div>
 
               <p class="post-category">Entertainment</p>
 
               <h2 class="title">
                 <a href="http://localhost:5173/postsdetail">2 ngày 1 đêm "Tự do, tự lo" mùa 2 | Tập 12</a> <button class="btn btn-outline-primary">Like</button> |
                 <button class="btn btn-outline-success">Share </button>
               </h2>
 
               <div class="d-flex align-items-center">
                 <img src="" alt="" class="img-fluid post-author-img flex-shrink-0">
                 <div class="post-meta">
                   <p class="post-author">Mark Dower</p>
                   <p class="post-date">
                     <time datetime="2022-01-01">Jun 22, 2022</time>
                   </p>
                 </div>
               </div>
               
             </article>
           </div><!-- End post list item -->
           <br><br>



           <div class="col-lg-12 col-md-12 col-sm-12" data-aos-delay="300">
             <article>
 
               <div class="post-img">
                 <img :src="imageUrl3" alt="" class="img-fluid">
               </div>
 
               <p class="post-category">Entertainment</p>
 
               <h2 class="title">
                 <a href="http://localhost:5173/postsdetail">2 ngày 1 đêm "Tự do, tự lo" mùa 2 | Tập 15</a> <button class="btn btn-outline-primary">Like</button> |
                 <button class="btn btn-outline-success">Share </button>
               </h2>
 
               <div class="d-flex align-items-center">
                 <img src="" alt="" class="img-fluid post-author-img flex-shrink-0">
                 <div class="post-meta">
                   <p class="post-author">Mark Dower</p>
                   <p class="post-date">
                     <time datetime="2022-01-01">Jun 22, 2022</time>
                   </p>
                  
                 </div>
               </div>
 
             </article>
           </div><!-- End post list item -->
 

 
 
   </template>
   
   <script>
   export default {
    data() {
      return {
        imageUrl2: 'https://trungtamnhatngu.edu.vn/uploads/blog/2014_12/connan-nhatngusofl_1.jpg',
        imageUrl3: 'https://cdn.tuoitre.vn/471584752817336320/2023/9/28/kv-ngang-mua-2-them-text-1695876925190691477736.png',
        imageUrl4: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRSFRRxj3mjFFrJ4NzDB3NAPwTLBAda0kKU4A&s',
        imageUrl6: 'https://gcs.tripi.vn/public-tripi/tripi-feed/img/474113qfT/hinh-anh-tu-nhien-dep-binh-di_014859861.jpeg'
    };
    },
  };
   </script>
   
   <style scoped>
   /* Định dạng container */
   .container {
     max-width: 1200px;
     margin: 0 auto;
     flex-wrap: wrap;  /* Cho phép các phần tử bẻ xuống hàng mới */
     padding: 0 15px;  /* Đảm bảo có padding cho các thiết bị nhỏ */
   }
   
   /* Căn giữa và chỉnh khoảng cách cho tiêu đề */
   .section-title {
     text-align: center;
     margin-bottom: 3rem;
   }
   
   /* Đảm bảo rằng ảnh hiển thị đúng */
   .post-img img {
     width: 100%;
     height: auto;
     border-radius: 8px;
     object-fit: cover;  /* Đảm bảo ảnh không bị méo */
   }
   
   /* Điều chỉnh kiểu hiển thị của danh mục bài viết */
   .post-category {
     font-size: 14px;
     color: #ff7e5f; /* Đổi màu danh mục */
     margin-bottom: 10px; /* Thêm khoảng cách dưới danh mục */
   }
   
   /* Cập nhật kiểu dáng tiêu đề bài viết */
   .title a {
     font-size: 20px;
     font-weight: bold;
     color: #333; /* Màu chữ tiêu đề mặc định */
     text-decoration: none;
     display: block;
     margin: 10px 0;
   }
   
   /* Thêm hiệu ứng hover cho tiêu đề */
   .title a:hover {
     color: #ff7e5f; /* Màu chữ hover */
     text-decoration: underline; /* Thêm underline khi hover */
   }
   
   /* Điều chỉnh kiểu ảnh tác giả và khoảng cách */
   .post-author-img {
     width: 30px;
     height: 30px;
     border-radius: 50%;
     margin-right: 10px;
     object-fit: cover; /* Đảm bảo ảnh tác giả không bị méo */
   }
   
   /* Cập nhật kiểu hiển thị của meta thông tin bài viết */
   .post-meta p {
     margin: 0;
     font-size: 14px;
     color: #6c757d; /* Màu chữ meta */
   }
   
   /* Điều chỉnh màu sắc của thời gian */
   .post-date time {
     color: #888; /* Màu chữ thời gian */
   }
   
   /* Kiểu dáng cho các nút */
   .btn-outline-primary {
     color: #ff7e5f;
     border: 1px solid #ff7e5f;
   }
   
   .btn-outline-primary:hover {
     background-color: #ff7e5f;
     color: #fff;
   }
   
   .btn-outline-success {
     color: #feb47b;
     border: 1px solid #feb47b;
   }
   
   .btn-outline-success:hover {
     background-color: #feb47b;
     color: #fff;
   }
   
   /* Phản hồi với màn hình nhỏ */
   </style>
   
   