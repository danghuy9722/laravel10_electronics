1. Tạo file migration
php artisan make:migration create_tests_table
2. Đồng bộ file migration
php artisan migrate
3. Xóa file file migration
php artisan migrate:rollback
4. Cập nhật file .env
php artisan config:cache
5. tạo dữ liệu mẫu
php artisan db:seed
6. tạo dữ liệu mẫu và reset toàn bộ
php artisan migrate:fresh --seed
7. Tạo controller
php artisan make:controller TestController
8. Tạo model
php artisan make:model Flight
10. thêm đoạn này vào để fix lỗi không nhận controller trong RouteServiceProvider
protected $namespace = 'App\Http\Controllers';
11. tạo file request
php artisan make:request StudentRequest
12. Tạo ra từng seed riêng ứng với db
php artisan make:seeder UserSeeder
13. Sử dụng factory để tạo dữ liệu mẫu
php artisan make:factory StudentsFactory --model=Students
14. Link ảnh
php artisan storage:link
15. tạo controler resouce 
php artisan make:controller ProductController --api 
php artisan make:resource ProductResource 
php artisan route:list --name=products
16. Xóa toàn bộ bảng
php artisan migrate:rollback
16. autoload
composer dump-autoload