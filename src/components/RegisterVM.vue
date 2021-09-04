<template>
    <div>
        <form action="/" @submit.prevent="sended()"> 
      <!-- <div class="row mt2">
        <div class="col-md-6">
        </div>
      </div> -->
      <div class="container p-5">
        <div class="card shadow">
          <div class="card-header">Virtual Machine Registration</div>
          <div class="card-body">
            <div class="row g-1">
                <div class="col-md-6">
                  <label for="virtualmachinename">Virtual Machine Name</label>
                  <input class="form-control" type="text" name="virtualmachinename" ref="virtualmachinename" id="virtualmachinename" placeholder="Virtual Machine Name">
                </div>
                <div class="col-md-6">
                  <div>
                    <input class="form-control" type="radio" name="environment" ref="environment" id="environment" placeholder="environment" checked>
                <label for="production">Production</label>
                  </div>
                  <div>
                <input class="form-control" type="radio" name="environment" ref="environment" id="environment" placeholder="environment" checked>
                <label for="development">development</label>                
                </div>
            <div class="row">
              <div class="col-md-6">
                <label for="duration">duration</label>
                <input class="form-control" type="number" name="duration" ref="duration" id="duration" placeholder="duration">
              </div>
              </div>
              <div class="row">
                <div class="col-md-6">
                  <label for="application">application</label>
                  <input class="form-control" type="number" name="application" ref="application" id="application" placeholder="application">
                </div>
              </div>
              <div class="row">
                <div class="col-md-6">
                  <label for="port">port</label>
                  <input class="form-control" type="number" name="port" ref="port" id="port" placeholder="port">
                </div>
                <div class="col-md-6">
                  <label for="incomingoutgoing">Incoming/Outgoing</label>
                  <input class="form-control" type="text" name="incomingoutgoing" ref="incomingoutgoing" id="incomingoutgoing" placeholder="incomingoutgoing">
                </div>
              </div>
              <div class="row">
                <div class="col-md-6">
                <label for="sourceip">sourceip</label>
                <input class="form-control" type="text" name="sourceip" ref="sourceip" id="sourceip" placeholder="sourceip">
              </div>
            </div>
            <div class="row p-3">
                <div class="col-md-6">
                  <label for="destinationip">destinationip</label>
                  <input class="form-control" type="text" name="destinationip" ref="destinationip" id="destinationip" placeholder="destinationip">
</div>
            <div class="row p-3">
                <div class="col-md-6">
                  <label for="os">os</label>
                  <input class="form-control" type="os" name="os" ref="os" id="os" placeholder="os">
                </div>
            </div>

                <div class="col-md-12">
                  <label for="program">program</label>
                  <input class="form-control" type="textarea" name="program" ref="program" id="program" placeholder="program">
                </div>
            </div>
            <div class="row">
<div class="row p-3">
            <div>
                <div class="col-md-6">
                  <label for="recipients">recipients</label>
                  <input class="form-control" type="text" name="recipients" ref="recipients" id="recipients" placeholder="recipients">
                </div>
            </div>            
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                            <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="internetaccess">Confirm Password</label>
                  <input class="form-control" type="number" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="cpu">cpu</label>
                  <input class="form-control" type="number" name="cpu" ref="cpu" id="cpu" placeholder="cpu">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="partition">partition</label>
                  <input class="form-control" type="text" name="partition" ref="partition" id="partition" placeholder="partition">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="size">size</label>
                  <input class="form-control" type="number" name="size" ref="size" id="size" placeholder="size">
                </div>
                </div>
            </div>

            <div class="row">
              <div class="col-md-6">
              </div>
              <div class="col-md-6">
                <button class="btn btn-outline-primary mr-3">Create Virtual Machine</button> 
                <!--&nbsp-->
                <input type="reset" class="btn btn-outline-danger" name="" id="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    </form>
    </div>
</template>
<script>
import axios from 'axios'
export default {
    name:"VirtualMachineRegistration",
    methods:{
    sended(){
      var environment = this.$refs.environment.value
      var duration = this.$refs.duration.value
      var application = this.$refs.application.value
      var port = this.$refs.port.value
      var incomingoutgoing = this.$refs.incomingoutgoing.value
      var sourceip = this.$refs.sourceip.value
      var destinationip = this.$refs.destinationip.value
      var program = this.$refs.program.value
      var os = this.$refs.os.value
      var recipients = this.$refs.recipients.value
      var internetaccess = this.$refs.internetaccess.value
      var datacenter = this.$refs.datacenter.value
      var backuprequired = this.$refs.backuprequired.value
      var pip = this.$refs.pip.value
      var status = this.$refs.status.value
      var project = this.$refs.project.value
      var  osarchitecture= this.$refs.osarchitecture.value
      var ram = this.$refs.ram.value
      var cpu  = this.$refs.cpu.value
      var partition  = this.$refs.partition.value
      var  size = this.$refs.size.value
      var vmtype   = this.$refs.vmtype.value
      var monitoringrequired   = this.$refs.monitoringrequired.value
      var author = this.$refs.author.value
      var date = this.$refs.date.value
      //var  = this.$refs..value
      //var q = document.getElementById("gender").value
      console.log(virtualmachinename,ownername,ownermobilenumber, ownermobilenumber,owneremailid,lf,lfemailid,lfmobilenumber,city, pincode, address, password, confirmpassword)
      axios.post('http://localhost:3000/data',{virtualmachinename:virtualmachinename, ownername:ownername, ownermobilenumber:ownermobilenumber, owneremailid:owneremailid, lf:lf, lfemailid:lfemailid, 
      lfmobilenumber:lfmobilenumber, city:city, pincode:pincode, address:address, password:password, confirmpassword:confirmpassword})
      .then(res => {
            console.log(res.data);
        })
    }
  }, 
}
</script>
