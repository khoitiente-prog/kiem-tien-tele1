let xu = 0;

function watchAd() {
  alert("Đang hiển thị video quảng cáo...");
  setTimeout(() => {
    xu += 10;
    document.getElementById("xu").textContent = xu;
    alert("🎉 Bạn đã nhận được 10 xu!");
  }, 3000); // giả lập xem video 3s
}

function withdraw() {
  if (xu >= 100) {
    alert("Gửi yêu cầu rút tiền tới bot Telegram...");
    xu -= 100;
    document.getElementById("xu").textContent = xu;
    // Gửi yêu cầu đến Telegram Bot của bạn
    fetch(`https://api.telegram.org/bot8092552054:AAF89UHQY8TbGZsAUfTRdnJpCJdtAyZoYH8/sendMessage?chat_id=@kiemxungon_bot&text=🧲 Người dùng vừa rút 100 xu!`)
      .then(() => alert("✅ Đã gửi yêu cầu rút tiền!"))
      .catch(err => alert("Lỗi gửi yêu cầu đến bot!"));
  } else {
    alert("❌ Bạn cần ít nhất 100 xu để rút tiền.");
  }
}
