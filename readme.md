# Benutzung

```bash
cd ansible_test
make
```

# Zugangsdaten für die Systeme der Laborumgebung

```bash
In diesem Testszenario können Sie sich auf allen Maschinen mit dem Benutzer ansible
anmelden, das Passwort ist ebenfalls ansible . Das Root-Account erreichen Sie auf den
Maschinen centos und suse via su , auf allen anderen via sudo . Das Root-Passwort (falls
erforderlich) ist ebenfalls ansible .
```

# Falls Probleme auftreten

```bash
Leider funktioniert die Software Vagrant nicht immer völlig sorgenfrei, vor allem in Kombination mit VirtualBox. 
Sollten bei Ihnen gewisse VMs nicht anständig provisioniert werden oder sich erst gar
nicht starten lassen (das scheint mitunter von der Tagesform oder der Mondphase
abzuhängen), so hilft oft ein erneuter Versuch:
$ vagrant reload <VM_NAME>
```

# Ansible-Installation auf dem Control Host

```bash
Auf einem die Windows-Testsysteme hatte die suse -VM Probleme, die auch damit nicht zu beheben waren. 
Hier half ein
$ vagrant plugin install vagrant-vbguest

$ vagrant up suse
```