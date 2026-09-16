# ChaeChae-C.github.io
<div class="copy-box">
    <pre>오늘 뭐 먹을지 골라주는 앱 만들어줘.</pre>
    <button class="copy-btn">⧉ 복사하기</button>
</div>

<div class="copy-box">
    <pre>추석에 가족과 함께 하는 윷 던지기 앱을 만들어줘.</pre>
    <button class="copy-btn">⧉ 복사하기</button>
</div>

<script>
document.querySelectorAll('.copy-btn').forEach(button => {
    button.addEventListener('click', async () => {
        const text = button.previousElementSibling.innerText;

        await navigator.clipboard.writeText(text);

        const original = button.innerText;
        button.innerText = '✓ 복사되었습니다';

        setTimeout(() => {
            button.innerText = original;
        }, 1500);
    });
});
</script>
