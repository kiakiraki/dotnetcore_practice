## プロジェクトの新規作成

```text
> dotnet new console -o hello_world

.NET Core 3.0 へようこそ!
---------------------
SDK バージョン: 3.0.100

テレメトリ
---------
.NET Core ツールは、エクスペリエンスの向上のために利用状況データを収集します。データは匿名です。
データは Microsoft によって収集され、コミュニティと共有されます。テレメトリをオプトアウトするに 
は、好みのシェルを使用して、DOTNET_CLI_TELEMETRY_OPTOUT 環境変数を '1' または 'true' に設定でき 
ます。

.NET Core CLI ツールのテレメトリの詳細をご覧ください: https://aka.ms/dotnet-cli-telemetry       

----------------
ドキュメントを確認する: https://aka.ms/dotnet-docs
問題を報告し、GitHub でソースを参照する: https://github.com/dotnet/core
新機能を参照する: https://aka.ms/dotnet-whats-new
インストール済みの HTTPS 開発者の証明書の詳細情報: https://aka.ms/aspnet-core-https
'dotnet --help' を使用して利用可能なコマンドを確認するか、次にアクセスする: https://aka.ms/dotnet-cli-docs
初めてのアプリを作成する: https://aka.ms/first-net-core-app
Getting ready...
The template "Console Application" was created successfully.

Processing post-creation actions...
Running 'dotnet restore' on hello_world\hello_world.csproj...
  G:\work\sandbox\dotnet\dotnetcore_practice\hello_world\hello_world.csproj の復元が 53.13 ms で完了しました。

Restore succeeded.

> cd .\hello_world\
```

## プログラムの実行

```text
> dotnet run
Hello World!
```

## プログラムの編集

```cs
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
            Console.WriteLine("The current time is " + DateTime.Now);   // 追記
        }
    }
```

```text
> dotnet run
Hello World!
The current time is 2019/11/11 14:41:52
```
