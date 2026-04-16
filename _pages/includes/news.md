# 🔥 News

<div class="news-scroll" id="news-scroll" role="region" aria-label="Recent news" data-visible-items="8" style="overflow-y: auto;">
  <ul>
    <li>2026.04: 🎉 Four papers are accepted by ACL 2026 (Main)</li>
    <li>2026.01: 🎉 One paper is accepted by CVPR 2026</li>
    <li>2025.09: 🎉 One paper is accepted by NeurIPS 2025</li>
    <li>2025.09: 🎉 Our <a href="https://arxiv.org/pdf/2408.08921">GraphRAG</a> survey is accepted by TOIS</li>
    <li>2025.05: 🎉 Two papers are accepted by ACL 2025 (Main)</li>
    <li>2025.02: 🚩 Our team ranked the 5-th position (5/76) in the <a href="https://tsinghua-fib-lab.github.io/AgentSocietyChallenge/pages/recommendation-track.html">AgentSociety Challenge</a> [Topic: Agent for Recommendation]</li>
    <li>2025.01: 🎉 Two papers are accepted by WWW 2025</li>
    <li>2024.12: 🧑🏻‍🏫 Invited talk on GraphRAG at 🕸️<a href="https://ldbcouncil.org/event/nineteenth-tuc-meeting/">LDBC</a></li>
    <li>2024.11: 🎉 One paper is accepted by KDD 2025</li>
    <!-- <li>2024.10: 📘 Our <a href="https://arxiv.org/abs/2410.10329">Graph Foundation Model</a> is available</li> -->
    <li>2024.09: 🎉 One paper is accepted by EMNLP 2024 (Main)</li>
    <!-- <li>2024.08: 📘 The first survey of <a href="https://arxiv.org/pdf/2408.08921">GraphRAG</a> is available!</li> -->
    <!-- <li>2024.07: 📘 First time as corresponding author for two papers: <a href="https://arxiv.org/pdf/2407.19420">UniGAP</a> and <a href="https://arxiv.org/abs/2408.07654">DeGTA</a></li> -->
    <li>2024.07: 🚩 Our team ranked the 3-rd position (3/508) in the <a href="https://www.aicrowd.com/challenges/amazon-kdd-cup-2024-multi-task-online-shopping-challenge-for-llms">KDD CUP 2024</a> [Topic: LLMs for Recommendation]</li>
    <!-- <li>2024.06: 📘 Our new work named <a href="https://arxiv.org/pdf/2406.12608">GraphBridge</a> is available</li> -->
    <li>2024.04: 🎉 One paper is accepted by IJCAI 2024</li>
    <!-- <li>2024.01: 🎈 We release <a href="https://github.com/ZhuYun97/ENGINE">ENGINE</a></li> -->
    <!-- <li>2024.01: 📘 Chinese blog of <a href="https://zhuanlan.zhihu.com/p/680351601">GraphControl</a> is available</li> -->
    <!-- <li>2024.01: 🎈 We release <a href="https://github.com/wykk00/GraphControl">GraphControl</a> and <a href="https://github.com/ZhuYun97/MARIO">MARIO</a></li> -->
    <li>2024.01: 🎉 Two papers are accepted by WWW 2024</li>
    <li>2023.07: 🎉 One paper is accepted by ECAI 2023</li>
    <li>2023.04: 🎉 One paper is accepted by IJCAI 2023</li>
    <li>2022.04: 🎉 One paper is accepted by IJCAI 2022</li>
  </ul>
</div>

<script>
  (function () {
    function updateNewsHeight() {
      var container = document.getElementById("news-scroll");
      if (!container) return;

      var visibleItems = parseInt(container.getAttribute("data-visible-items"), 10) || 8;
      var items = container.querySelectorAll("li");

      if (items.length <= visibleItems) {
        container.style.height = "auto";
        container.style.overflowY = "visible";
        return;
      }

      var previousScrollTop = container.scrollTop;
      container.scrollTop = 0;

      var targetItem = items[visibleItems - 1];
      var containerRect = container.getBoundingClientRect();
      var targetRect = targetItem.getBoundingClientRect();
      var computedStyle = window.getComputedStyle(container);
      var paddingBottom = parseFloat(computedStyle.paddingBottom) || 0;
      var borderBottom = parseFloat(computedStyle.borderBottomWidth) || 0;
      var height = Math.ceil(targetRect.bottom - containerRect.top + paddingBottom + borderBottom);

      container.style.height = height + "px";
      container.style.overflowY = "auto";
      container.scrollTop = previousScrollTop;
    }

    document.addEventListener("DOMContentLoaded", updateNewsHeight);
    window.addEventListener("load", updateNewsHeight);
    window.addEventListener("resize", updateNewsHeight);
  })();
</script>
