# Viet-Hoa-QBCORE
Đây Là Font Việt Hóa Của QBCORE
- Bước 1 : Mở qb-core/client/functions.lua
  + Dan Muc Sau Day Vao
   -- FONT VIỆT HÓA 
Citizen.CreateThread(function()
    RegisterFontFile('out')
    QBCore.Font = RegisterFontId('Baloo Paaji 2 SemiBold')
    AddTextEntry('STRING', "<FONT FACE = 'Baloo Paaji 2 SemiBold'>~a~</FONT>")
    AddTextEntry('CUSTOM_STRING', "<FONT FACE = 'Baloo Paaji 2 SemiBold'>~a~</FONT>")
end)

function QBCore.Functions.FloatingNotification(msg, x,y,z)
    AddTextEntry('FloatingNotification', "FONT FACE = 'Baloo Paaji 2 SemiBold'>"..msg.."</FONT")
    SetFloatingHelpTextWorldPosition(1, x, y, z)
    SetFloatingHelpTextStyle(1, 1, 2, -1, 3, 0)
    BeginTextCommandDisplayHelp('FloatingNotification')
    EndTextCommandDisplayHelp(2, false, false, -1)
end
- Bước 2 : Trong Thư Mục qb-core Tạo Một Thư Mục Có Tên "stream" Và Dán Font Có Đuôi gfx Trong Đây Để Chạy KHai Báo
- Lưu Ý : Nếu Font Vẫn Lỗi Vui Lòng Thêm "<FONT FACE = 'Baloo Paaji 2 SemiBold'>" Đây Đọc Mã
          + Có Thể Áp Dụng Cho Cả ESX
