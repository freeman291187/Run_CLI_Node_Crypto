**TENEO
```console
(function autoClick() {
    // Sử dụng selector cho nút Connect Node
    const targetSelector = 'button.bg-blue-teneo.rounded.w-full.text-sm.mt-1.text-white.p-3';
    const checkInterval = 5000; // Kiểm tra mỗi 5 giây

    function checkAndClick() {
        const button = document.querySelector(targetSelector);
        if (button) {
            console.log("Tìm thấy nút Connect Node!");
            
            // Nếu nội dung của button không phải "Connect Node" (tức là bị disconnect) thì click
            if (button.innerText.trim() !== "Disconnect Node") {
                console.log("Trạng thái không phải 'Connect Node', đang click để kết nối lại...");
                button.click();
            } else {
                console.log("Trạng thái là 'Connect Node', không cần click.");
            }
        } else {
            console.log("Không tìm thấy nút Connect Node.");
        }
    }

    setInterval(checkAndClick, checkInterval);
})();
```
