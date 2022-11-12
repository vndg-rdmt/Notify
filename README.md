# Notify

Custom visual console for web development.

## Usage

Import Notiy and initiate first custom console.

```js
import Notify from "..." //Entry point is notify/index.ts

const MyConsole = Notify.initConsole({
    id: 'Debug',
    historySize: 10,
    logger: true, 
});

MyConsole.display();

// id: string - Displayed name. More for semantic.
// historySize: number - Maximum logs, displayed in one time.
// logger?: boolean - If true - will write logs you can later export. Default - false.
// interfaceId? --- currently unavailable ---. It's changing console view interface. Default - 'terminal'.

// .display() mounts element to DOM (Just makes it visible, logs and messages are still working even it don't mounted). it can take a parameter - custom mount point. By default it's document.body.
```
Your first console will appear on the page. You can create any amount of consoles.
Consoles are fully draggble, you can put them in any place on the page by dragging them by the title part of the console.

![Снимок экрана 2022-11-12 в 16 46 25](https://user-images.githubusercontent.com/118057254/201477439-fb154a49-2f29-41f6-a350-d67b79ef2f92.png)

## Interface

There are two buttons - minimize view and clear history.

**Minimize view** will hide history but not clear it. History is still will receive messages and write logs.

![Снимок экрана 2022-11-12 в 16 46 38](https://user-images.githubusercontent.com/118057254/201477848-5e4f4d8f-9f3a-4137-8a21-ef2264c268e6.png)

**Clear history** deletes all elements from the history.

![Снимок экрана 2022-11-12 в 16 46 59](https://user-images.githubusercontent.com/118057254/201477944-23c2e381-82b4-4e54-bd48-7810d58a780e.png) ![Снимок экрана 2022-11-12 в 16 46 25](https://user-images.githubusercontent.com/118057254/201478046-86fe9020-2512-4c00-a2b0-72ec2929aa3f.png)


