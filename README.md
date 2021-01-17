# HelloXBOX

## 準備 (Prepare)

### Visual Studio 
- UWPコンポーネントをインストールしておく (Install UWP component)
    - デフォルトでは C++ が含まれないので注意 (By default C++ is not included)
### PC
- 開発者モードを有効化しておく (Enable developer mode)
    - 設定(Settings) - 更新とセキュリティ(Update and security) - 開発者向け(For developer) - 開発者モード(Developer mode)

### アカウント (Account)
- [開発者アカウントを登録 (Register developer account)](https://developer.microsoft.com/ja-jp/store/register/)
- 開発者プログラムへ参加するには$19かかる (It costs $19 to participate developer program)

## 手順
- 【XBOX】Dev Mode Activation アプリをダウンロードする (On XBOX, download Dev Mode Activation application)
    - アプリを起動、画面にコードが表示される (Invoke application, and code will be displayed)
- 【PC】 https://aka.ms/activatexbox へアクセス (From PC access https://aka.ms/activatexbox)
    - Dev devices - Xbox One development consoles - 右の「+」ボタン(Right side ”+" button) - Enter activation code - 上記のコードを入力 (Enter above code)
- 【XBOX】 Dev Mode Activation - Switch and restart で再起動、開発者モードへ (Restart and enter development mode)
    - リテールモードに戻すには (To return to retail mode) Home - Quick actions - Leave Dev Mode
    - ネットワーク設定をし、開発者アカウントでサインインする (Setup network, and sign in with developer account)
    - 右下の Remote Access に IP が表示されているので覚えておく (Right down, IP address is displayed)
- 【PC】プロジェクトを作成 (Create project)
    - Visual Studio - Create a new Project - DirectX 12 App   (Universal Windows-C++/CX)
    - プラットフォームを x64 にする (Select x64 platform)
    - プロジェクト右クリック(Right click project) - Debugging - Debugger to Launch で Remote Machine を選択 (Select Remote Machine) - Machine Name に上記IPを指定 (Specify IP address above)
    - Remote Machine で起動すると初回は PIN の入力を要求される (Invoke Remote Machine, need to input PIN on first time)
        - 【XBOX】Home - Quick Actions - Show Visual Studio pin - でPINが表示できるので Visual Studio へ入力する (PIN will displayed, input to Visual Studio)
- 【XBOX】
    - Game & Apps 以下に自作プログラムが現れる (Game & Apps section, there is my program) 
