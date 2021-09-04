<template>
    <div>
        <form action="/" >
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
                  <label for="internetaccess">Internet Access</label>
                  <input class="form-control" type="text" name="internetaccess" ref="internetaccess" id="internetaccess" placeholder="internetaccess">
                </div>
                </div>
            </div>
                            <div class="col-md-6">
                  <label for="datacenter">Data Center</label>
                  <input class="form-control" type="text" name="datacenter" ref="datacenter" id="datacenter" placeholder="datacenter">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="backuprequired">backup required?</label>
                  <input class="form-control" type="text" name="backuprequired" ref="backuprequired" id="backuprequired" placeholder="backuprequired">
                </div>
                </div>
            </div>
                <div class="col-md-6">
                  <label for="pip">PIP</label>
                  <input class="form-control" type="text" name="pip" ref="pip" id="pip" placeholder="pip">
                </div>
                </div>
            <div>
                <div class="col-md-6">
                  <label for="status">Status</label>
                  <input class="form-control" type="text" name="status" ref="status" id="status" placeholder="status">
                </div>
            </div>
            <div>
                <div class="col-md-6">
                  <label for="project">project</label>
                  <input class="form-control" type="text" name="project" ref="project" id="project" placeholder="project">
                </div>
                </div>
            <div>
                <div class="col-md-6">
                  <label for="osarchitecture">osarchitecture</label>
                  <input class="form-control" type="text" name="osarchitecture" ref="osarchitecture" id="osarchitecture" placeholder="osarchitecture">
                </div>
                </div>
            <div>
                <div class="col-md-6">
                  <label for="ram">ram</label>
                  <input class="form-control" type="number" name="ram" ref="ram" id="ram" placeholder="ram">
                </div>
                </div>
          <div>
                <div class="col-md-6">
                  <label for="cpu">cpu</label>
                  <input class="form-control" type="number" name="cpu" ref="cpu" id="cpu" placeholder="cpu">
                </div>
            </div>
            <div>
                <div class="col-md-6">
                  <label for="partition">partition</label>
                  <input class="form-control" type="number" name="partition" ref="partition" id="partition" placeholder="partition">
                </div>
                </div>
         <div>
                <div class="col-md-6">
                  <label for="size">size</label>
                  <input class="form-control" type="number" name="size" ref="size" id="size" placeholder="size">
                </div>
                </div>
           <div>
            <div class="row">
              <div class="col-md-6">
              </div>
             <div class="col-md-6">
                <button class="btn btn-outline-primary mr-3">Create Virtual Machine</button> 
                <input type="reset" class="btn btn-outline-danger">
              </div>
            </div>
          </div>
    </form>
</div>
</template>
<script>
export default {
    name:"VirtualMachineRegistration",
   }
</script>
