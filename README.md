[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyeo11200&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
  
![Anurag's github stats](https://github-readme-stats.vercel.app/api?username=yeo11200&show_icons=true&theme=radical)

name: Update gist with WakaTime stats
on:
  schedule:
    - cron: "0 0 * * *"
jobs:
  update-gist:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@master
      - name: Update gist
        uses: matchai/waka-box@master
        env:
          GH_TOKEN: 28dcdd1f-4d2e-4c3d-9ff4-bfd023461484
          GIST_ID: 968220c97e8da1d047a9a480fa432e54
          WAKATIME_API_KEY: 7dd9b32a-b8bd-4207-a4ec-46b8fd7f13c8
