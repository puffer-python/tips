Welcome, you guys, to contribute your tips to everyone by creating a pull request [![GitHub issues](https://img.shields.io/github/issues/puffer-python/tips)](https://github.com/puffer-python/tips/issues)
## Linux
### RUN cmds in a file 

```cmd
while read p; do   bash -c  "$p"; done < tet.ok
```
## GIT
### Delete all local branches except a branch

```cmd
git branch | grep -v "master" | grep -v "branch_1" | xargs git branch -D
```

### CURL

```python
import asyncio
import aiohttp


async def fetch_url(session, url):
    async with session.get(url) as response:
        print(f"URL: {url}, Status: {response.status}")


async def do_curl(urls):
    async with aiohttp.ClientSession() as session:
        tasks = [fetch_url(session, url) for url in urls]
        await asyncio.gather(*tasks)


if __name__ == "__main__":
    asyncio.run(do_curl([
        "https://"
    ]))

```
