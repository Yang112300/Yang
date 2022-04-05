# Yang
测试
Public Class Form1

    Private Sub Button1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles Button1.Click
        Try
            SerialPort1.Open() '打开串口
            Label2.Text = SerialPort1.IsOpen
            If SerialPort1.IsOpen = True Then
                Label1.Text = "串口已连接"
                Label1.ForeColor = Color.Green
            End If
        Catch ex As Exception
            '    MessageBox.Show(ex.Message)
        End Try

    End Sub
